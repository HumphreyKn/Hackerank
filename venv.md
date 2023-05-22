# Python Virtual Environments

A virtualenv (AKA venv) is essentially a Virtual Machine (VM) or sandbox environment that runs an independent and untouched Python environment.

When you create and activate the venv you no longer have access to the main Python environment running on your system.
The problem programmers have is that it can be hard to isolate problems in code when their primary environment is cluttered with imported modules and the like.
Best practice would be to create a venv within your project and use it to run your project.

## Creating Virtual Environments

Before creating a venv, install virtualenv using: `pip inatall virtualenv`.
Let’s create a venv called `awesome-test`. You’d preferably run the following commands in your project root dir:

- Unix Commands

``` python
python3 -m venv awesome-test
ls
# awesome-text
```

- Windows Commands

``` python
python -m venv awesome-test
dir
#awesome-test
```

## Activating the venv

Activating the venv puts you into a standalone Python instance that has pretty much nothing installed by default:

- Unix Commands

``` python
cd awesome-test
ls
bin     include     lib     pyvenv.cfg
#
# source bin/activate
(awesome-test) #
(awesome-test) # echo YAY!
YAY!
```

- Windows commands

```python
cd awesome-test
dir
#Include/    Lib/    pyvenv.cfg  Scripts/
 Scriptsactivate
#(awesome-test) #
#(awesome-test) # echo YAY!
#YAY!
```

The `awesome-test` tag preceding your shell prompt indicates you’re now in the venv.

Now list out the modules installed in this python instance:

```python
# pip list
pip (9.0.1)
setuptools (28.8.0)
#
```

If you’ve been using Python already, you’ll know that your main env would have a boat load of modules installed. It’s nice to be able to run from a clean slate when desiging new code!

You can now play around and install whatever the heck you want without having to worry about corrupting or screwing up your primary environment. All modules installed in this venv will remain local to the venv.

When you’re done using the venv you then exit (deactivate) it using the `deactivate` command:

- **Unix Command**

```python
(awesome-test) # deactivate
#
```

- **Windows Command**

```python
(awesome-test) # Scriptsdeactivate
#
```

**Note:** _All of changes you made in the venv will NOT be lost. It’s all stored safely within the venv._

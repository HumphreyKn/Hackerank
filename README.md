# Python If-Else

## Task
Given an integer `n`, perform the following conditional actions:
    - if `n` is odd, print `Wierd`
    - if `n` is even and in the inclusive range of 2 to 5, print `Not Wierd`
    - if `n` is even and in the inclisuve range of 6 to 20, print `Wierd`
    - If `n` is even and greater than 20, print `Not Wierd`

### Input format
A single line containing a positive integer `n`.

### Constraints
$$1\leq n \leq 100$$

### Output fotmat
Print `Wierd` if the number is wierd. Otherwise print `Not Wierd`.

### Sample Inputs and Outputs
#### Sample input 0

```
3
```
#### Sample output 0

```
3
```
#### Explanation 0
$n=3$
`n` is odd and odd numbers are wierd, so print `Wierd`.

#### Sample input 1

```
24
```
#### Sample output 1

```
Not Wierd
```
#### Explanation 1

$n=24$
$n>20$ and `n` is even, so it is not wierd.

# sol_calc

## intro
simple calcaulator

<img src="./img/test_sol_calc">

## Usage
### install
```
$ pip install sol_calc
```
### python code
```python
from sol_add.add import add
from sol_mul.mul import mul
from sol_div.div import div

import sys
x = int(sys.argv[1])
y = int(sys.argv[2])

def a():
    add(x, y)

def m():
    mul(x, y)

def d():
    div(x, y)
```
### add pyproject.toml option
```
dependencies = ["sol_add>=0.1.0", "sol_mul>=0.1.0", "sol_div>=0.1.0"]

[project.scripts]
sol-add = "sol_calc.calc:a"
sol-mul = "sol_calc.calc:m"
sol-div = "sol_calc.calc:d"
```

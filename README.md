## This is a py file

pytest is a Python testing framework used to automatically test your code.

**Basic example**

Suppose you have:

#### calculator.py
`def add(a, b):`
    `return a + b`

Create:

#### test_calculator.py
`from calculator import add`


`def test_add():`
    `assert add(2, 3) == 5`

Then run:

`pytest`

pytest finds files like test_*.py automatically and runs functions beginning with test_.

#### Useful commands
`pytest`

Run all tests.

`pytest test_calculator.py`

Run one test file.

`pytest -v`

Verbose output.

`pytest -k "add"`

Run tests whose names contain add.

`pytest -x`

Stop at the first failure.

#### Install
`pip install pytest`

The key idea is:

**You write assert statements describing what your code should do → pytest runs them and tells you what passes/fails.**
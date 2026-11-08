# PLP - Python-week-6 Assignment
## Safe Functions with try / except

Submitted for: Python-Week-6 - Catching Errors

### Files in this Repository
- **safe_tools.py** - Contains the three required functions: safe_divide, safe_number, and get_field. Each function uses try/except so the program does not crash on bad or unwise input.
- **README.md** - This file, describing the assignment and answering the reflection question.

### Program Output
When safe_tools.py is run, it produces the following output:

5.0
Cannot divide by zero
42
Not a number
82
Field not found

### Reflection Question: Why can the if check not catch abc on its own?

An if check cannot catch "abc" on its own because the error happens during the conversion itself. When Python runs int("abc"), it raises a ValueError immediately, before any if statement can check the result. For this reason, only try/except can catch the error and allow the program to continue running.
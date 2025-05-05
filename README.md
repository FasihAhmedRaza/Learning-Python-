### Python Interview Questions for Beginners (with Simple Explanations + Examples)

**1. Difference between Module and Package?**

* **Module:** Python file (e.g., `math.py`)
* **Package:** Folder with `__init__.py` and modules inside.

```python
# module: math_utils.py
# package: utils/
```

**2. Python compiled ya interpreted?**

* Interpreted hai (line by line run hota hai).

**3. Python ke benefits?**

* Easy syntax, ML/AI libraries, huge community, automation ke liye best.

**4. Global, Protected, Private attributes?**

```python
class A:
    x = 1         # public
    _y = 2        # protected
    __z = 3       # private
```

**5. Python case sensitive hai?**

* Yes. `name != Name`

**6. Pandas kya hai?**

* Data handling ke liye library hai:

```python
import pandas as pd
```

**7. Exception handling kaise?**

```python
try:
    x = 1 / 0
except ZeroDivisionError:
    print("Error")
```

**8. For loop vs While loop?**

```python
for i in range(3): print(i)
i = 0
while i < 3:
    print(i)
    i += 1
```

**9. Indentation required?**

* YES! Python me white space important hai.

**10. self kya karta hai?**

* Current object ko refer karta hai:

```python
class A:
    def __init__(self, x):
        self.x = x
```

---

### Intermediate Python Interview Questions

**11. Python memory manage kaise karta hai?**

* Reference counting + garbage collection

**12. Multiple inheritance support hai?**

* Yes.

```python
class A: pass
class B: pass
class C(A, B): pass
```

**13. Memory management?**

* Automatic via garbage collector

**14. File delete kaise karte hain?**

```python
import os
os.remove("file.txt")
```

**15. sort() vs sorted()?**

* `sort()` list ko change karta hai; `sorted()` naya list deta hai.

**16. List vs Tuple?**

* List = mutable, Tuple = immutable

**17. Slicing in Python?**

```python
l = [1,2,3,4,5]
print(l[1:4])  # [2,3,4]
```

**18. Multithreading kaise hoti hai?**

```python
from threading import Thread
```

**19. List vs NumPy Array?**

* NumPy faster hoti hai due to C-based backend.

**20. Inheritance explain?**

```python
class Parent: pass
class Child(Parent): pass
```

**21. Class kaise banate hain?**

```python
class MyClass:
    def __init__(self):
        print("Hello")
```

**22. Fibonacci series?**

```python
a, b = 0, 1
for _ in range(5):
    print(a)
    a, b = b, a + b
```

**23. Shallow vs Deep Copy?**

```python
import copy
copy.copy()  # shallow
copy.deepcopy()  # deep
```

**24. Compilation & Linking?**

* Python bytecode banata hai (`.pyc`), linking manually nahi hoti.

**25. break, continue, pass?**

```python
for i in range(5):
    if i == 2: continue  # skip
    if i == 4: break     # stop
    pass  # do nothing
```

**26. PEP8 kya hai?**

* Python coding style guide

**27. Expression kya hai?**

* Code jo value return kare:

```python
x = 2 + 3
```

**28. == kya karta hai?**

* Value compare karta hai (not memory).

**29. Type conversion?**

```python
x = int("5")  # string to int
```

**30. Common Python Modules?**

* `os`, `math`, `random`, `json`, `datetime`

```python
import math
print(math.sqrt(16))
```

---

### Advanced Python Interview Questions

**31. xrange vs range?**

* Python 2 me `xrange()` hota tha (lazy iterator), Python 3 me sirf `range()` hai.

**32. zip function kya karta hai?**

* Lists ko pair karta hai:

```python
zip([1,2], ['a','b'])  # [(1,'a'), (2,'b')]
```

**33. Django architecture?**

* MTV (Model-Template-View)

**34. Inheritance (repeat):**

```python
class A: pass
class B(A): pass
```

\*\*35. \*args and **kwargs?**

```python
def f(*args, **kwargs):
    print(args)
    print(kwargs)
```

**36. Runtime errors example?**

```python
print(10 / 0)  # ZeroDivisionError
```

**37. Docstrings kya hain?**

* Function/class/documentation ke liye:

```python
def f():
    """This is docstring"""
```

**38. Capitalize first letter?**

```python
"hello".capitalize()  # Hello
```

**39. Generators kya hain?**

* `yield` use kar ke iterator banate hain:

```python
def gen():
    yield 1
    yield 2
```

**40. Comment kaise likhte hain?**

```python
# This is a comment
```

**41. GIL kya hai?**

* Global Interpreter Lock: Ek thread ek time me run karta hai.

**42. Django vs Flask?**

* Django: Full framework
* Flask: Lightweight, flexible

**43. Flask kya hai? Benefits?**

* Web framework, fast prototyping, lightweight

**44. PIP kya hai?**

* Python package manager:

```bash
pip install numpy
```

**45. Python 2 & 3 compatibility?**

* Use `__future__`, `six` module, compatible syntax likhna

**46. %, /, // difference?**

```python
5 % 2  # 1 (modulus)
5 / 2  # 2.5 (division)
5 // 2 # 2 (floor division)
```

**47. Python memory deallocation kyun nahi karta?**

* OS handle karta hai. Interpreter kuch references hold kar leta hai.

**48. Set unordered kyu? Mutable hai?**

* Order guarantee nahi. Haan, mutable hota hai.

**49. DataFrame vs Series?**

* DataFrame = table (rows + columns)
* Series = single column

**50. len() kya karta hai?**

* Length return karta hai:

```python
len([1,2,3])  # 3
```

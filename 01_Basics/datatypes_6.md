Type Casting – int()

int():

=> int() is used to convert one type of value into int type value

=> Syntax:
   varname = int(value)

🟡 Example-1: float → int (Possible)

=> a = 12.34
=> print(a, type(a))   → 12.34 <class 'float'>

=> b = int(a)
=> print(b, type(b))   → 12 <class 'int'>

=> a = 0.5
=> b = int(a)
=> print(b)   → 0

🟡 Example-2: bool → int (Possible)

=> a = True
=> b = int(a)
=> print(b)   → 1

=> a = False
=> b = int(a)
=> print(b)   → 0

❌ Example-3: complex → int (Not Possible)

=> a = 2+3j
=> b = int(a)   → TypeError

🟡 Example-4: str → int
Case-1: valid integer string (Possible)

=> a = "12"
=> b = int(a)
=> print(b)   → 12 <class 'int'>

❌ Case-2: float string (Not Possible)

=> a = "12.34"
=> b = int(a)   → ValueError

❌ Case-3: boolean string (Not Possible)

=> a = "True"
=> b = int(a)   → ValueError

❌ Case-4: pure string (Not Possible)

=> a = "PYTHON"
=> b = int(a)   → ValueError





🎯 Type Casting – float()

float():

=> float() is used to convert one type of value into float type value

=> Syntax:
   varname = float(value)

🟡 Example-1: int → float (Possible)

=> a = 100
=> print(a, type(a))   → 100 <class 'int'>

=> b = float(a)
=> print(b, type(b))   → 100.0 <class 'float'>

=> a = 0
=> b = float(a)
=> print(b)   → 0.0

🟡 Example-2: bool → float (Possible)

=> a = True
=> b = float(a)
=> print(b)   → 1.0

=> a = False
=> b = float(a)
=> print(b)   → 0.0

❌ Example-3: complex → float (Not Possible)

=> a = 2+3j
=> b = float(a)   → TypeError

🟡 Example-4: str → float
Case-1: integer string (Possible)

=> a = "12"
=> b = float(a)
=> print(b)   → 12.0 <class 'float'>

Case-2: float string (Possible)

=> a = "12.34"
=> b = float(a)
=> print(b)   → 12.34 <class 'float'>

❌ Case-3: invalid float string

=> a = "12.34.45"
=> b = float(a)   → ValueError

❌ Case-4: boolean string

=> a = "True"
=> b = float(a)   → ValueError

❌ Case-5: complex string

=> a = "2+3j"
=> b = float(a)   → ValueError

❌ Case-6: pure string

=> a = "Python3.11"
=> b = float(a)   → ValueError




🎯 Type Casting – bool()

bool():

=> bool() is used to convert value into boolean type

=> Syntax:
   varname = bool(value)

=> Rule:
   non-zero / non-empty → True
   zero / empty → False

🟡 Example-1: int → bool (Possible)

=> a = 123
=> b = bool(a)
=> print(b)   → True

=> a = 0
=> b = bool(a)
=> print(b)   → False

🟡 Example-2: float → bool (Possible)

=> a = 12.34
=> b = bool(a)
=> print(b)   → True

=> a = 0.0
=> b = bool(a)
=> print(b)   → False

🟡 Example-3: complex → bool (Possible)

=> a = 2+3j
=> b = bool(a)
=> print(b)   → True

=> a = 0+0j
=> b = bool(a)
=> print(b)   → False

🟡 Example-4: str → bool (Important)

=> a = "123"
=> bool(a)   → True

=> a = "True"
=> bool(a)   → True

=> a = " "
=> bool(a)   → True

=> a = ""
=> bool(a)   → False

⭐ Important Points

- 0, 0.0, 0+0j → False
- "" (empty string) → False
- any non-zero / non-empty → True



🎯 Type Casting – complex()

complex():

=> complex() is used to convert value into complex type

=> Syntax:
   varname = complex(value)

🟡 Example-1: int → complex (Possible)

=> a = 12
=> b = complex(a)
=> print(b)   → (12+0j)

🟡 Example-2: float → complex (Possible)

=> a = 3.4
=> b = complex(a)
=> print(b)   → (3.4+0j)

🟡 Example-3: bool → complex (Possible)

=> a = True
=> b = complex(a)
=> print(b)   → (1+0j)

=> a = False
=> b = complex(a)
=> print(b)   → 0j

🟡 Example-4: str → complex (Limited)

=> a = "2+3j"
=> b = complex(a)
=> print(b)   → (2+3j)

❌ Example-5: invalid string

=> a = "python+3j"
=> b = complex(a)   → ValueError

⭐ Important Points

- result format → (a + bj)
- real part + imaginary part
- bool → True=1, False=0
- valid complex string only allowed

⭐ Interview
👉 complex(10) → (10+0j)
👉 complex("2+3j") → valid






🎯 Type Casting – str()

str():

=> str() is used to convert any type of value into string type

=> Syntax:
   varname = str(value)

🟡 Example-1: int → str (Possible)

=> a = 123
=> b = str(a)
=> print(b, type(b))   → 123 <class 'str'>

=> b → "123"

🟡 Example-2: float → str (Possible)

=> a = 23.45
=> b = str(a)
=> print(b, type(b))   → 23.45 <class 'str'>

=> b → "23.45"

🟡 Example-3: bool → str (Possible)

=> a = True
=> b = str(a)
=> print(b, type(b))   → True <class 'str'>

=> b → "True"

🟡 Example-4: complex → str (Possible)

=> a = 2.5+6.7j
=> b = str(a)
=> print(b, type(b))   → (2.5+6.7j) <class 'str'>

=> b → "(2.5+6.7j)"

⭐ Important Points

- str() converts everything into string
- result always in quotes form
- no error in conversion

⭐ Interview
👉 str(10) → "10"
👉 str(True) → "True"


Hey 👋  
You can find the complete DataTypes-6 Class notes in PDF format below 👇

👉 [Click here to view/download Variables Notes](datatypes-6.pdf)


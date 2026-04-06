DATA-TYPES
The purpose of DT in PYTHON is that "To allocate Sufficient Amount of Memory Space in main Memory of Computer and inputs can stored".

 
Data Types in Python:

Fundamental Types:
- int   → integer (10)
- float → decimal (10.5)
- bool  → True / False

Sequence Types:
- str   → string ("Aman")

Collection Types (Data Structures):
- list
- tuple
- set
- dict

Fundamental Data Types:

-To Strore the Single Value
- int   → integer (10)
- float → decimal (10.5)
- bool  → True / False

int (Integer):

- stores whole numbers (no decimal)
int is used to store integer (whole) numbers without decimal values.
- example: 10, 123, -5

a = 123
print(a)
print(type(a))

Notes:
Built-in names:

- int, str, list are predefined names in Python
- can be used as variable names but not recommended

Example:
int = 34 # not recommended but correct


Number Systems in int:

- Python supports different number systems to represent integers
- Decimal → base 10 (10)
- Binary  → base 2 (0b1010)
- Octal   → base 8 (0o12)
- Hexa    → base 16 (0xA)


Note-
👉 type() ka use hota hai:
➡️ ye check karne ke liye ki variable kis type ka hai
Ex:
a = 10
print(type(a))
<class 'int'>

 name="aman"
Print(type(name))
<class 'str'>




Number Systems in Python:

Decimal:
- base 10 (0–9)
- default number system

Binary:
- base 2 (0,1)
- prefix: 0b
- example: 0b1010

Important:
- Python converts all number systems into decimal internally
- all are stored as int


Conversion:
- bin() → decimal to binary
- example: bin(10) → 0b1010

#Binary To Decimal
a=0b1101
print(a)




Python internally converts all number systems into decimal.


Octal Number System:

- base 8 (digits: 0–7)
- prefix: 0o

Important:
- digits 8 and 9 are not allowed
- Python converts octal to decimal internally
- stored as int

Example:
0o33 → 27
![Uploading image.png…]()

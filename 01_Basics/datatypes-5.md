
Full slicing:

- syntax: str[:]
- no begin, no end specified
- returns complete string

🧠 UNDERSTANDING

begin → default 0
end → default len(string)
👉 Matlab:

str[:] = str[0:len(str)]

💻 Examples

s = "PYTHON"

print(s[:])     # PYTHON
print(s[0:])    # PYTHON
print(s[:6])    # PYTHON
print(s[0:6])   # PYTHON


s = "JAVA PROG"

print(s[:])           # JAVA PROG
print(s[0:len(s)])    # JAVA PROG
print(s[-len(s):])    # JAVA PROG

⭐ Important

- [:] always returns full string
- no error even if range not given



🎯 STRING SLICING WITH STEP (FINAL NOTES)
✅ Ye padh (must)

Slicing with step:

- syntax: str[begin:end:step]
- step controls direction & gap

🟡 RULE 1 (MOST IMPORTANT)

step > 0 → left to right
step < 0 → right to left

🟡 CASE 1: step = +ve

s = "PYTHON"

print(s[0:4:1])   # PYTH
print(s[0:6:2])   # PTO
print(s[0:6:3])   # PH
print(s[::1])     # PYTHON
👉 Rule:

begin < end hona chahiye, warna "" (empty)

🟡 CASE 2: step = -ve (reverse)

s = "PYTHON"

print(s[::-1])    # NOHTYP
print(s[5:0:-1])  # NOHTY
print(s[5:2:-1])  # NOH
👉 Rule:

begin > end hona chahiye

🟡 CASE 3: wrong range

print(s[2:1])     # "" ❌
print(s[1:3:-1])  # "" ❌

🧠 VISUAL

P   Y   T   H   O   N
0   1   2   3   4   5
-6 -5 -4 -3 -2 -1

⭐ Special (important)

print("PYTHON"[::-1])   # reverse ✔
print("MOM"[::-1]) == "MOM"   # True (palindrome)




🧠 SIMPLE MEANING

str[begin : end : step]
👉 step = jump size

✅ CASE 1

print(s12[0:4:1])
👉 step = 1
➡️ har index pe jao (no jump)

0 → P  
1 → Y  
2 → T  
3 → H
👉 Output: PYTH

✅ CASE 2

print(s12[0:6:2])
👉 step = 2
➡️ 1 character skip karo (jump by 2)

0 → P  
2 → T  
4 → O
👉 Output: PTO

🎯 FINAL RULE (WRITE THIS)

step = 1 → no skipping
step = 2 → skip 1 character
step = 3 → skip 2 characters

🔥 SHORT FORMULA

jump = step
skip = step - 1



🎯 MUTABLE vs IMMUTABLE (FINAL NOTES)
✅ Mutable (can change)

Mutable:

- values can be modified after creation
- same object (memory) update hota hai
- no new object created (mostly)

Examples:
list, set, dict, bytearray

💻 Examples

# list
a = [1, 2, 3]
a[0] = 10
print(a)   # [10, 2, 3]

# set
s = {1, 2, 3}
s.add(4)
print(s)

# dict
d = {"a": 1}
d["a"] = 100
print(d)

✅ Immutable (cannot change)

Immutable:

- values cannot be modified after creation
- any change creates new object
- original value remains same

Examples:
int, float, bool, str, tuple, complex

💻 Examples

# string
s = "Aman"
# s[0] = "R"   ❌ Error

# int
a = 10
a = 20   # new object created

# tuple
t = (1, 2, 3)
# t[0] = 10   ❌ Error
➡️ Immutable = value same, reference change
🟡 Important Points

- mutable → direct change possible
- immutable → change means new object
- strings are immutable (VERY IMPORTANT)



Hey 👋  
You can find the complete DataTypes-5 Class notes in PDF format below 👇

👉 [Click here to view/download Variables Notes](datatypes-5.pdf)


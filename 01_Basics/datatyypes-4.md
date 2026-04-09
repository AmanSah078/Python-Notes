🎯 STRING OPERATIONS (FINAL NOTES)
✅ Ye padh (must)

1.Indexing:

- used to access single character from string
- syntax: str[index]
- index can be +ve (left to right) or -ve (right to left)

🟡 Important

- +ve index starts from 0
- -ve index starts from -1
- invalid index → IndexError

🧠 VISUAL

P   Y   T   H   O   N
0   1   2   3   4   5   → +ve

-6 -5 -4 -3 -2 -1       → -ve


💻 Examples (cover all types)

s = "PYTHON"

print(s[0])    # P
print(s[1])    # Y
print(s[5])    # N

print(s[-1])   # N
print(s[-2])   # O
print(s[-6])   # P

print(s[3])    # H
print(s[-3])   # H

💻 Boundary + Error

s = "MISSISSIPPI"

print(s[len(s)-1])   # last character
print(s[0])          # first character

print(s[len(s)])     # ❌ IndexError


//Let's Try To Understand
🎯 CLEAR EXPLANATION

s = "MISSISSIPPI"
👉 Length:

len(s) = 11

🧠 STEP-BY-STEP
✅ Last character

print(s[len(s)-1])
👉 = s[11-1] = s[10]
👉 Output:

I
✔ Correct (last index = 10)

✅ First character

print(s[0])
👉 Output:

M
✔ Always first index = 0

❌ Error case

print(s[len(s)])
👉 = s[11]
❌ ERROR:

IndexError
👉 Kyun?
➡️ Last index = 10
➡️ Tu access kar raha hai 11

🎯 SIMPLE RULE (NOTE)

Last index = len(s) - 1
len(s) is out of range

💬 FINAL
👉 Valid index: 0 → 10
👉 Invalid: 11 ❌

⭐ Interview
👉 indexing starts from 0
👉 negative indexing allowed
👉 invalid index → error

🎯 STRING SLICING (FINAL NOTES)
✅ Ye padh (must)

Slicing:

- used to get substring from string
- syntax: str[begin:end]
- begin included, end excluded

🧠 VISUAL (VERY IMPORTANT)

P   Y   T   H   O   N
0   1   2   3   4   5
-6 -5 -4 -3 -2 -1

🟡 CASE 1: str[begin:end]

s = "PYTHON"

print(s[0:3])   # PYT
print(s[2:6])   # THON
print(s[1:6])   # YTHON
print(s[2:1])   # "" (no result)
print(s[0:6])   # PYTHON

🟡 CASE 2: negative slicing

print(s[-6:-2])   # PYTH
print(s[-3:-1])   # HO
print(s[-6:-3])   # PYT
print(s[-3:-6])   # "" (invalid range)
print(s[-6:-1])   # PYTHO

🟡 CASE 3: mix (+ve , -ve)

print(s[1:-2])   # YTH
print(s[2:-1])   # THO

🟡 CASE 4: only begin
It means Remove From Begin
Aage se 2 Remove
print(s[2:])   # THON
print(s[0:])   # PYTHON
print(s[3:])   # HON

🟡 CASE 5: only end
Piche se 2 Remove
print(s[:2])   # PY
print(s[:4])   # PYTH

🟡 EDGE CASES (IMPORTANT)

print(s[12:44])   # "" (out of range safe)
print(s[-66:-1])  # PYTHO
print(s[2:2])     # "" (same index)
Notes: If index is out of range, Python adjusts it to valid range which is 0
⭐ RULES (IMPORTANT)

- begin included, end excluded
- if begin > end → empty string ""
- slicing never gives error (safe)
- supports negative indexing




<img width="633" height="4219" alt="image" src="https://github.com/user-attachments/assets/5cfa7e47-16d9-49ca-9849-a515c9d59e32" />

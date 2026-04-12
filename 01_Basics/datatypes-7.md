🎯 4. range()

range:

=> range() is used to generate sequence of integer values

=> it is immutable (cannot modify values)

=> mainly used in loops
=>On the object of range,we can perform Both indexing slicing operations
Ex=> r1=range(1,10) //0 1 2 3 4 5 6 7 8 9
 print(r1,(type(r1)),id(r1))
For v1 in r1:
R1[1]=>4


🟡 Syntax-1: range(value)

=> varname = range(value)

=> generates values from 0 to value-1

=> r = range(6)
=> output → 0 1 2 3 4 5

🟡 Syntax-2: range(begin, end)

=> varname = range(begin, end)

=> generates values from begin to end-1

=> r = range(10,16)
=> output → 10 11 12 13 14 15
Only -1 from the end dude

🟡 Syntax-3: range(begin, end, step)

=> varname = range(begin, end, step)

=> generates values with step interval

=> r = range(10,21,2)
=> output → 10 12 14 16 18 20

💻 Loop Example (IMPORTANT)

for i in range(6):
    print(i)


for i in range(10,16):
    print(i, end=" ")
# 10 11 12 13 14 15

⭐ Important Points

- end value is always excluded
- default step = 1
- works in forward direction

⭐ Interview
👉 range(5) → 0 to 4
👉 range(2,6) → 2 to 5



🟡 Backward (Reverse Range)

=> for backward direction step must be negative (-ve)

=> begin > end hona chahiye

💻 Example-1

for i in range(5, 0, -1):
    print(i)

Output → 5 4 3 2 1

💻 Example-2

for i in range(10, 5, -1):
    print(i)

Output → 10 9 8 7 6

💻 Example-3

for i in range(6, -1, -1):
    print(i)

Output → 6 5 4 3 2 1 0

⭐ Important

- step negative → reverse direction
- begin must be greater than end
- end still excluded

- Hey 👋  
You can find the complete DataTypes-7 Class notes in PDF format below 👇

👉 [Click here to view/download Variables Notes](datatypes-7.pdf)








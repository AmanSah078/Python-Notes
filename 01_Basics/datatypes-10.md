🎯 Nested List (Inner List)

Nested List:

=> ek list ke andar dusri list ho to usse nested list kehte hain

🧠 REAL EXAMPLE (TERE IMAGE WALA)

lst = [100, "Karthik", [18,16,20], [76,75,66], "OUCET"]

🔍 BREAKDOWN

Outer list:
[100, "Karthik", [...], [...], "OUCET"]

Inner lists:
[18,16,20]
[76,75,66]

🎯 ACCESS KARNA (VERY IMPORTANT 🔥)
🟡 Outer elements

print(lst[0])   # 100
print(lst[1])   # Karthik
print(lst[-1])  # OUCET

🟡 Inner list access

print(lst[2])   # [18,16,20]
print(lst[3])   # [76,75,66]

🟡 Inner ke andar ka element

print(lst[2][0])   # 18
print(lst[2][1])   # 16
print(lst[3][2])   # 66

💥 MODIFY (IMPORTANT)

lst[2][1] = 17
print(lst)
# [100, 'Karthik', [18,17,20], [76,75,66], 'OUCET']

🧠 GOLDEN RULE (WRITE THIS 🔥)

nested list access:

lst[i][j]

i → outer index  
j → inner index

🎯 REAL LIFE CONNECTION

Student data:

[Roll, Name, [internal marks], [external marks], college]








🎯 del Operator (VERY IMPORTANT 🔥)

del:

=> used to delete elements or entire object

🟡 Syntax-1: delete by index

=> del objname[index]

=> removes element at given index


lst = [10, "Sagatika", 66.66, "OUCET", "HYD"]

del lst[-2]
print(lst)
# [10, 'Sagatika', 66.66, 'HYD']

🟡 Syntax-2: delete using slicing

=> del objname[begin:end:step]

=> removes multiple elements


lst = [10, "Sagatika", 66.66, "OUCET", "HYD"]

del lst[0:2]
print(lst)
# [66.66, 'HYD']


lst = [10, "Sagatika", 66.66, "OUCET", "HYD"]

del lst[::2]
print(lst)
# ['Sagatika', 'OUCET']

🟡 Syntax-3: delete entire object

=> del objname

=> deletes whole variable


lst = [10, "Sagatika"]

del lst

print(lst)   # ❌ NameError

🧠 Important Points

- del removes element or variable
- supports index and slicing
- deleting variable → NameError on access
- list object changes (mutable)




🎯 Pre-defined Function in List → index()

index():

=> used to find index of first occurrence of given value

=> Syntax:
   listobj.index(value)

🟡 Example

lst = [10,20,30,40,10,60,70]

print(lst)
# [10,20,30,40,10,60,70]


print(lst.index(10))   # 0
print(lst.index(20))   # 1
print(lst.index(30))   # 2

🟡 Duplicate Case (IMPORTANT 🔥)

lst = [10,20,30,40,10]

print(lst.index(10))   # 0 (first occurrence only)

❌ Error Case

lst.index(300)   # ❌ ValueError (not present)


[].index(10)   # ❌ ValueError

🧠 Important Points

- returns index of FIRST occurrence
- works based on VALUE
- if value not found → ValueError




🎯 Copy Techniques → Shallow Copy

Shallow Copy:

=> used to create a copy of list

=> Syntax:
   list2 = list1.copy()

🟡 Properties of Shallow Copy

a) initial content of both objects same

b) memory address of outer objects different

c) modifications in outer elements are independent

d) inner (nested) objects share same reference ❗

💻 Example-1 (Simple List)

lst1 = [10, "Rossum", 34.56]
lst2 = lst1.copy()

print(lst1)
print(lst2)


lst1.append("PYTHON")

print(lst1)   # [10, 'Rossum', 34.56, 'PYTHON']
print(lst2)   # [10, 'Rossum', 34.56]
👉 ✔ change reflect nahi hua  ->sirf dude phla hi na change hua dusara thodi na hua dude

💻 Example-2 (Nested List 🔥)

lst1 = [10, [20, 30]]
lst2 = lst1.copy()

lst2[1][0] = 999

print(lst1)   # [10, [999, 30]] ❗
print(lst2)
👉 ❗ change reflect hua

🧠 Important Points

- outer list → new object
- inner list → same reference
- simple values → safe
- nested values → shared

⭐ Quick Revision

Shallow Copy:

outer → new  
inner → same




🎯 FINAL TRUTH (WRITE THIS 🔥)

lst2 = lst  → no copy

- same object
- same memory
- change in one → reflect in both

👉 Step 1

lst = [10, "Aman", 34.56]
lst2 = lst

id(lst) == id(lst2) ✔

👉 Step 2

lst.append("PYTHON")
👉 Output:

lst  → [10, 'Aman', 34.56, 'PYTHON']
lst2 → [10, 'Aman', 34.56, 'PYTHON'] ❗
➡️ dono change hue

👉 Step 3

lst.remove("Aman")
👉 Output:

lst  → [10, 34.56, 'PYTHON']
lst2 → [10, 34.56, 'PYTHON'] ❗
➡️ again dono change



🎯 Pre-defined Function in List → count()

count():

=> used to count number of occurrences of given value in list

=> Syntax:
   listobj.count(value)

🟡 Example

lst = [10,20,30,10,20,50,60,70,10]

print(lst)
# [10,20,30,10,20,50,60,70,10]


print(lst.count(10))   # 3
print(lst.count(20))   # 2
print(lst.count(30))   # 1


print(lst.count(40))   # 0 (not present)
print(lst.count("PYTHON"))   # 0


print([].count(10))   # 0

🧠 Important Points

- counts occurrences of value
- returns integer
- if value not found → 0 (no error)




🎯 Pre-defined Function in List → reverse()

reverse():

=> used to reverse elements of list (in-place)

=> Syntax:
   listobj.reverse()

🟡 Example-1

lst1 = [10, "Rossum", 34.56, "PYTHON"]
print(lst1)


lst1.reverse()
print(lst1)
# ['PYTHON', 34.56, 'Rossum', 10]

🟡 Example-2

lst2 = [10,20,30,100,200,300]

lst2.reverse()
print(lst2)
# [300,200,100,30,20,10]

🟡 Return Value (IMPORTANT 🔥)

lst = [1,2,3]

x = lst.reverse()
print(x)   # None


print([1,2,3].reverse())   # None

🧠 Important Points

- reverses list in-place (same object)
- does NOT create new list
- returns None

⭐ Quick Revision Line

reverse = reverse list (same object)




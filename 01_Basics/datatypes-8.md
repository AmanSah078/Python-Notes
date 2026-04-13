🎯 LIST (FINAL NOTES)
✅ Properties of List

=> list is a pre-defined class (list data type)

=> used to store multiple values (same or different types)

=> allows duplicate values

=> elements are stored in square brackets [ ]

=> elements separated by comma

=> maintains insertion order

=> supports indexing and slicing

=> list is mutable (can modify)

🟡 Types of List
a) Empty List

=> contains no elements
=> length = 0

=> Syntax:
   varname = []
   (OR)
   varname = list()

b) Non-Empty List

=> contains elements
=> length > 0

=> Syntax:
   varname = [val1, val2, ..., valn]
   (OR)
   varname = list(object)

💻 Examples (VERY IMPORTANT)
✅ Basic List

l1 = [10, 20, 30]
print(l1, type(l1))   # [10, 20, 30] <class 'list'>

✅ Mixed Data Type

l2 = [20, "Rossum", 34.56, True, 2+3j]
print(l2, type(l2))

✅ Indexing

l2 = [20, "Rossum", 34.56, True, 2+3j]

print(l2[0])    # 20
print(l2[1])    # Rossum
print(l2[-1])   # (2+3j)

✅ Slicing

print(l2[1:4])    # ['Rossum', 34.56, True]
print(l2[0:5:2])  # [20, 34.56, (2+3j)]
print(l2[::-1])   # reverse

✅ Mutable (change possible)

l2 = [20, "Rossum", 34.56, True]

l2[0] = 100
print(l2)   # [100, 'Rossum', 34.56, True]

✅ Length

l1 = [10, "Rossum", 34.56]
print(len(l1))   # 3

l2 = []
print(len(l2))   # 0

✅ Empty List

l2 = []
print(l2, type(l2), len(l2))   # [] <class 'list'> 0

l3 = list()
print(l3)   # []

✅ list() with iterable

s = "MISSISSIPPI"
l = list(s)
print(l)
# ['M','I','S','S','I','S','S','I','P','P','I']

✅ bytes → list

l1 = [10,20,30,40,50,60]
b = bytes(l1)
l2 = list(b)
print(l2)   # [10,20,30,40,50,60]

❌ Error Case

x = 100
b = list(x)   # ❌ TypeError (not iterable)

✅ Fix

b = list([x])
print(b)   # [100]

⭐ Important Points

- list is mutable
- supports indexing & slicing
- allows duplicate values
- works with iterable only


🎯 Pre-defined Function in List → append()

append():

=> used to add element at the end of list

=> Syntax:
   listobj.append(value)

🟡 Example

lst = [10, "Rossum", 34.56]
print(lst, id(lst))


lst.append("PYTHON")
print(lst)
# [10, 'Rossum', 34.56, 'PYTHON']


lst.append(True)
print(lst)
# [10, 'Rossum', 34.56, 'PYTHON', True]


lst.append(1+2.5j)
print(lst)
# [10, 'Rossum', 34.56, 'PYTHON', True, (1+2.5j)]

🧠 Important

- adds only ONE element at a time
- element always added at END
- list id remains same (mutable)



🎯 Pre-defined Function in List → insert()

insert():

=> used to add element at specific index in list

=> Syntax:
   listobj.insert(index, value)

🟡 Example

lst1 = [10, "Karan", 34.56]
print(lst1, type(lst1))


lst1.insert(10, "python")   # invalid +ve index
# inserted at END


lst1.insert(-11, "java")    # invalid -ve index
# inserted at BEGINNING


print(lst1, type(lst1))
# ['java', 10, 'Karan', 34.56, 'python']

🧠 Important Points (ADD THIS 🔥)

- insert(index, value)

- if index > length → inserted at END
- if index < -length → inserted at BEGINNING

- elements shift after insertion
- list remains same object (mutable)

⭐ Quick Summary

valid index → exact position
large +ve index → end
large -ve index → start




🎯 Pre-defined Function in List → clear()

clear():

=> used to remove all elements from list

=> Syntax:
   listobj.clear()

🟡 Example

lst = [10, "Rossum", 34.56]
print(lst, id(lst), len(lst))


lst.clear()
print(lst, id(lst), len(lst))
# []  (same id, length = 0)

🟡 Empty List Case

lst = []
lst.clear()   # no error
print(lst)    # []

🟡 Return Value

lst = [1,2,3]

print(lst.clear())   # None


print([1,2,3].clear())   # None

🧠 Important Points

- removes all elements
- list becomes empty []
- does not create new object (same id)
- returns None
- safe for empty list (no error)


🎯 Pre-defined Function in List → remove()

remove():

=> used to remove first occurrence of given value from list

=> Syntax:
   listobj.remove(value)

🟡 Example-1 (Basic)

lst = [10, "Rossum", 34.56, "Python"]
print(lst, len(lst))


lst.remove("Rossum")
print(lst)   # [10, 34.56, 'Python']


lst.remove(34.56)
print(lst)   # [10, 'Python']


lst.remove("Python")
print(lst)   # [10]


lst.remove(10)
print(lst)   # []

❌ Error Case

lst.remove("Python")   # ❌ ValueError (not present)


[].remove(100)   # ❌ ValueError

🟡 Example-2 (Duplicate Values 🔥)

lst1 = [10,20,30,10,30,"Python",True]
print(lst1)


lst1.remove(10)
print(lst1)
# removes FIRST 10 only


lst1.remove(30)
print(lst1)
# removes FIRST 30 only

🧠 Important Points

- removes only FIRST occurrence
- works based on VALUE (not index)
- if value not found → ValueError




🎯 Pre-defined Function in List → pop(index)

pop():

=> used to remove element based on index

=> Syntax:
   listobj.pop(index)

🟡 Example-1 (Basic)

lst1 = [10,20,30,10,30,"Python",True]
print(lst1)


lst1.pop(3)
print(lst1)
# [10, 20, 30, 30, 'Python', True]


lst1.pop(-4)
print(lst1)
# removes element using negative index


lst1.pop(0)
print(lst1)
# removes first element


lst1.pop(0)
print(lst1)


lst1.pop(0)
print(lst1)

🟡 Return Value (IMPORTANT 🔥)

lst = [10,20,30]

x = lst.pop(1)
print(x)   # 20 (removed value)

🟡 Default Behavior

lst = [1,2,3]

lst.pop()   # removes last element
print(lst)  # [1,2]

❌ Error Case

lst = []
lst.pop()   # ❌ IndexError


lst = [1,2,3]
lst.pop(10)   # ❌ IndexError

🧠 Important Points

- removes element using index
- returns removed value
- default removes last element
- invalid index → IndexError

⭐ Quick Revision Line

pop = delete by index + returns value


🎯 Pre-defined Function in List → pop()

pop():

=> used to remove LAST element of list

=> Syntax:
   listobj.pop()

🟡 Example

lst = [10, "Rossum", 34.56, "Python"]
print(lst)


lst.pop()
print(lst)
# [10, 'Rossum', 34.56]


lst.pop()
print(lst)
# [10, 'Rossum']


lst.pop()
print(lst)
# [10]


lst.pop()
print(lst)
# []

❌ Error Case

lst.pop()   # ❌ IndexError (empty list)


[].pop()   # ❌ IndexError

🧠 Important Points

- removes last element
- no index required
- returns removed value
- empty list → IndexError


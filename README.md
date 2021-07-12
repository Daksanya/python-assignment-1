# python-assignment-1
#List program

list1=[1,2,2.3,4.5,"Daksha","Akshaya","ch",2,1]
list2=[5,6,7]
list1.append("sita")
print(list1)
x=list1.count(2)
print(x)
y=list1.copy()
print(y)
list1.extend(list2)
print(list1)
z=list1.index("Daksha")
print(z)
list1.pop(5)
print(list1)
list1.remove("Daksha")
print(list1)
list1.reverse()
print(list1)
list2.sort(reverse=True)
print(list2)
list1.clear()
print(list1)


#Tuple program

tuple1=(1,2,'Kavi','Tanu',2)
tuple2=(5,6,7)
print(tuple1)
x=tuple1.count(2)
print(x)
y=tuple1.index('Tanu')
print(y)

#Set Program

set1={1,2,'Ram','suriya'}
set2={5,6,7,'Ram'}
set1.add(5)
print(set1)
set1.pop()
print(set1)
set1.remove(2)
print(set1)
x=set1.copy()
print(x)
c=set1.isdisjoint(set2)
print(c)
d=set1.issubset(set2)
print(d)
e=set1.issuperset(set2)
print(e)
a=set1.intersection(set2)
print(a)
b=set1.intersection_update(set2)
print(b)
y=set1.difference(set2)
print(y)
z=set1.difference_update(set2)
print(z)
set1.discard(2)
print(set1)

#Dictionary program


dict1={"Name":"Monish","Dept":"CSE","college":"IITM"}
x=dict1.copy()
print(x)
a=('a','b','c')
b=0
dict2=dict.fromkeys(a,b)
print(dict2)
y=dict1.get("college")
print(y)
z=dict1.items()
print(z)
c=dict1.keys()
print(c)
dict1.pop('Dept')
print(dict1)
dict1.popitem()
print(dict1)
dict3={"Name":"Monish","Dept":"CSE","college":"IITM"}
d=dict3.setdefault("Dept","ECE")
print(d)
dict3.update({"Year":"2020"})
print(dict3)
e=dict3.values()
print(e)

#Calculator program

def add(x, y):
    return x + y
def subtract(x, y):
    return x - y
def multiply(x, y):
    return x * y
def divide(x, y):
    return x / y
print("Select operation.")
print("1.Add")
print("2.Subtract")
print("3.Multiply")
print("4.Divide")

while True:
    choice = input("Enter choice(1/2/3/4): ")
    if choice in ('1', '2', '3', '4'):
        num1 = float(input("Enter first number: "))
        num2 = float(input("Enter second number: "))

        if choice == '1':
            print(num1, "+", num2, "=", add(num1, num2))

        elif choice == '2':
            print(num1, "-", num2, "=", subtract(num1, num2))

        elif choice == '3':
            print(num1, "*", num2, "=", multiply(num1, num2))

        elif choice == '4':
            print(num1, "/", num2, "=", divide(num1, num2))
        break
    else:
        print("Invalid Input")

# python
 = int(input("Enter the Lower Range: "))
b = int(input("Enter the Upper Range: "))
c = 0
d = 0
if a > b:
    n = input("type Yes else No")
    if n == "Yes":
        temp = b
        b = a
        a = temp
for i in range(a, b+1):
    a = i
    n = 0
    for j in range(2, a):
        if a % j == 0:
            n = 1
            c += 1
            print(a, "is Composite Number")
            break
    if n == 0:
        print(a, "is Prime Number")
        d += 1
    if n == "No":
        pass
else:
    print("There are", d, "Prime numbers and,", c, "Composite numbers in the given range.")

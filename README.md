# HW4_2
#Variables
N = int(input("Number of Students: "))
counter =  0
A = 0
B = 0
C = 0
D = 0
E = ""
F = ""
G = ""
H = ""
#============================================================================
#main function
while counter < N:
    counter += 1
    grade = int(input("Score #%d : " % counter))
    if grade >= 87:
        A += 1
        E = "*" * A
    elif grade >= 75 and grade < 87:
        B += 1
        F = "*" * B
    elif grade > 65 and grade <75:
        C += 1
        G = "*" * C
    else:
        D += 1
        H = "*" * D

print("Grade   Frequency    Bar Chart")
print("    A","%11d"%A,"%4s"%E)
print("    B","%11d"%B,"%4s"%F)
print("    C","%11d"%C,"%4s"%G)
print("    D","%11d"%D,"%4s"%H)

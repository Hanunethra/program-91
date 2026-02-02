# program-91
row = int(input("Enter number of rows (even):"))

n = row//2

print("Generated butterfly pattern is:\n")
# Upper part
for i in range(1,n+1):
for j in range(1, 2*n+1):
if j&gt;i and j&lt; 2*n+1-i:
print("", end="")
else:
print("*", end="")
print()

# Lower part
for i in range(n,0,-1):
for j in range(2*n,0,-1):
if j&gt;i and j&lt; 2*n+1-i:
print(" "end="")
else:
print("*", end="")
print()
Output

Enter number of rows (even): 12
Generated butterfly pattern is:
* *
* * * *
* * * * * *
* * * * * * * *
* * * * * * * * * *
* * * * * * * * * * * *
* * * * * * * * * * * *
* * * * * * * * * *
* * * * * * * *
* * * * * *
* * * *
* *

import math
sieve=[]
n=100000001
for i in range(n):
    sieve.append(True)
    sieve[0]=sieve[1]=False
x=int(math.sqrt(n))
for i in range(2,x+1):
    if sieve[i]:
        for i in range(i*i,n,i):
            sieve[j]=False
m=int(input())
if sieve[m]:
    print(m)

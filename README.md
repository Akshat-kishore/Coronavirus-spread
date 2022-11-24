# Coronavirus-spread
t=int(input())
for i in range(t):
    n=int(input())
    x=list(map(int,input().split()))
    b=[]
    c=1
    for i in range(n-1):
        k=abs(x[i]-x[i+1])
        if k<=2:
            c+=1
        else:
            b.append(c)
            c=1
    b.append(c)
    print(min(b),max(b))
    
    #output: 
    #11
    #33
    #23

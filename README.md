# costliest-jwellery-set
n=int(input())
l=list(map(int,input().split()))
o=[]
o.append(max(l))
m=[]
for i in range(n-1):
    if l[i]<l[i+1]:
        m.append(l[i])
    else:
        m.append(l[i])
        o.append(sum(m))
        m=[]
m.append(l[-1])
o.append(sum(m))
print(max(o))

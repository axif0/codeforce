# codeforce
x,y=map(int,input().split())
nxtprime=0
list=[1,2,3,5,7]
for i in range(x+1,y+1):
    if i%2 !=0 and i%3!=0 and i%5!=0 and i%7!=0:
        nxtprime = i
        break
    if i in list:
        if i!=y:
            break
        elif i==y:
            nxtprime=i

if nxtprime==y :
    print("YES")
else:
    print("NO")

# python-dictionary-bytexl
# approach1
# sum of values of even keys
d={}
n=int(input())
for i in range(n):
  k,v=map(int,input().split())
  d[k]=v 
res=0
for i in d:
  if i%2==0:
    res=res+d[i]
print(res)

# approach2
# product values of odd keys
d={}
n=int(input())
for i in range(n):
  k,v=map(int,input().split())
  d[k]=v 
res=1 
for i in d:
  if i%2!=0:
    res=res*d[i]
print(res)

# approach3
d={}
n=int(input())
for i in range(1,n+1):
  d[i]=i+1 
print(d)

# approach4
d={}
n=int(input())
for i in range(1,n+1):
  if i%2!=0:
    d[i]=i*10
print(d)

# approach5
# sum of n natural numbers
d={}
n=int(input())
for i in range(1,n+1):
  res=0 
  for j in range(1,i+1):
    res=res+j 
  d[i]=res
print(d)

# approach6 factorial
d={}
n=int(input())
for i in range(1,n+1):
  res=1 
  for j in range(1,i+1):
    res=res*j 
  d[i]=res 
print(d)

# approach7 list in dictionaries & their factors
d={}
n=int(input())
for i in range(1,n+1):
  d[i]=[]
  for j in range(1,i+1):
    if i%j==0:
      d[i].append(j)
print(d)

# approach8
d={}
n=int(input())
for i in range(1,n+1):
  d[i]=[]
  for j in range(1,i+1):
    if i%j==0:
      d[i].append(j)
d1={}
for i in d:
  if len(d[i])>2:
    d1[i]="Not Prime"
  else:
    d1[i]="Prime"
print(d1)







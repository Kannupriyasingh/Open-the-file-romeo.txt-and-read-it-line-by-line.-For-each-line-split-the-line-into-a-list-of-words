# Open-the-file-romeo.txt
fname = input("Enter file name: ")
fh = open(fname)
lst = list()
for line in fh:
  l=line.rstrip()
  r=l.split()
  for i in r:
    if i not in lst:
      lst.append(i)
    else:
      continue
lst.sort() 
print(lst)    

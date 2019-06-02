import string

alll = string.printable[0:36] + string.printable[62:101] + " "

i = input()
i = i.lower()
c = 0

for position in range(69):
  for l in range(len(i)):
    if(alll[position] == i[l]):
      c += 1
    if(c != 0):
      print(100/len(i)*c,"% ",alll[position]," = ",c) 
  c = 0
		

# nestedlist
l1 = [[1,2,3],
      [11,12,'b','b','b'],
      [21,'t',223],
      [4,5,6],
      [7,8,9],
      'demo',
      12.5]
**if your nested list contains a string then find out its index and print it then remove them in the list**
for i in l1:
    if type(i) == list:
        j=0
        while j < len(i):
            if type(i[j]) is str:
                print("index of {} is".format(i[j]),j)
            j=j+1
        j=0
        while j < len(i):
            if type(i[j]) is str:
                i.remove(i[j])
                continue
            j=j+1
print("the list is",l1)
**Extract the second element of each nested list**
for i in l1:
    if type(i)==list:
        j=0
        while j<len(i):
            if j == 1:
                print("second element of {} nested list is ".format(i),i[j])
            j=j+1

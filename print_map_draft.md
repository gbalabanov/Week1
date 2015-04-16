with open("myfile.txt","w") as f:
    f.write("..S.$. ")
    f.write("!!..T. ")
    f.write(".....G")

arr=[]

with open("myfile.txt","r") as f:
    lines=f.read().split()
    for x in lines:
        arr.append(list(x))
    arr[0][0] = "S"
    print(arr)
    mine=(["".join(x) for x in arr])
    for x in mine:
        print(x,end="\n")

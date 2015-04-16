with open("myfile.txt","w") as f:
    f.write("H.....")
    f.write("\n")
    f.write("H!!..!")
    f.write("\n")
    f.write("H!T..!")
    
with open("myfile.txt","r") as f:
   text=f.read()
   
x=0
y=0
found=False
print(text)
text=text.split()
for row in text:
    for col in row:
        if col == "S":
            print(x,y)
            found=True
            break
        y+=1
    if found:
        break
    y=0
    x+=1


print(text[x][y])
print(text)

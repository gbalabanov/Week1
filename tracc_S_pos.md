with open("myfile.txt","r") as f:
   text=f.read()
   
x=0
y=0
print(text)
text=text.split()
for row in text:
    for col in row:
        if col == "S":
            print(x,y)
        x+=1
    y+=1

def is_palindrome(n):
    stringNum=str(n)
    if stringNum[::-1]==stringNum:
        return True
    else:
        return False

def hack_represent(n):
    x=n
    k=[]
    while (n>0):
        a=int(float(n%2))
        k.append(a)
        n=(n-a)/2
    k.append(0)
    string=""
    for j in k[::-1]:
        string=string+str(j)
    return string[1:]

def next_hack(n):
    hack_num=hack_represent(n)
    while True:
        if is_palindrome(hack_num):
            return n
        else:
            n+=1
            hack_num=hack_represent(n)

n=int(input('please enter the no. in decimal format: '))
print(next_hack(n));

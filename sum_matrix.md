def print_matrix(a,b):
    
    matrix=[[0 for x in range(b)] for x in range(a)]
    for i in range(a):
        for j in range(b):
            temp=int(input("Enter number: "))
            matrix[i][j]=temp
    print(matrix)
    return matrix

def sum_matrix(mtx):
    total=0
    for x in mtx:
        for j in x:
            total+=j
    return total

a=int(input("Enter rows"))
b=int(input("Enter cols"))
print(sum_matrix(print_matrix(a,b)))

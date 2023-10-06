 list_1 = [1, 'apple', 3, 'banana', 2, 'cherry']
n = len(list_1)
print(n)
i = 0
while i < n:
    if type(list_1[i]) == str:
        list_1.pop(i)
        n = n-1
        i = i - 1
    i = i + 1
print(list_1)
list_1.sort()
print(list_1)


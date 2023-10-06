 numbers = []
print(请输入三个整数x,y,z：)
for i in range(0, 3):
    numbers.append(int(input()))
print(numbers)
numbers.sort(reverse=True)
print(numbers)


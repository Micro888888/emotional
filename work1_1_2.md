numbers = []
print("请输入三个整数x,y,z：")
for i in range(0, 3):
    numbers.append(int(input()))
print(numbers)
numbers.sort()
maximum = max(numbers)
minimum = min(numbers)
numbers[0] = maximum
numbers[2] = minimum
print(numbers)

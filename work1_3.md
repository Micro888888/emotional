 str_1 = str(input(请输入一个字符串:))
# 字符串共n个字符
n = len(str_1)
print(n)
i = 0
# 定义布尔变量判断是否含有ol
b = False
# 字符串长度为1直接输出
if n == 1:
    print(f字符串为里面没有ol,这个字符串为：{str_1})
else:
    while i < n-1:
        if str_1[i] == o and str_1[i+1] == l:
            b = True
            str_1 = str_1[:i] + fzu + str_1[i+2:n]
            n = n+1
        i = i + 1
if b:
    print(n这个字符串里面有ol,修改后的字符串为：)
else:
    print(n这个字符串里面没有ol,原字符串为：)
print(str_1) 

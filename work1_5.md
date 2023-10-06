students_dict = {"112300123": "小张", "112300124": "小李",
                 "112300125": "小杜", "112200126": "小黄"}
# 字典在迭代过程中不可更改，故改为对列表进行操作
for i in list(students_dict.keys()):
    x = int(i)
    if x % 2 == 0:
        del(students_dict[i])
print(students_dict)



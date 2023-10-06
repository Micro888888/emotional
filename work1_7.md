class Product:
    # 初始化商品信息
    def __init__(self, product_number, product_name, unit_price, total_numbers, remaining_numbers):
        self.product_number = product_number
        self.product_name = product_name
        self.unit_price = unit_price
        self.total_numbers = total_numbers
        self.remaining_numbers = remaining_numbers

    # 显示商品信息
    def display(self):
        print(f"商品序号: {self.product_number}")
        print(f"商品名: {self.product_name}")
        print(f"单价: {self.unit_price}")
        print(f"总数量: {self.total_numbers}")
        print(f"剩余数量: {self.remaining_numbers}")

    # 计算已售出商品价值
    def income(self, sold_numbers):
        if sold_numbers <= self.remaining_numbers:
            value = sold_numbers * self.unit_price
            self.remaining_numbers -= sold_numbers
            return value
    # 修改商品信息

    def setdata(self, product_name, unit_price, total_numbers, remaining_numbers):
        self.product_name = product_name
        self.unit_price = unit_price
        self.total_numbers = total_numbers
        self.remaining_numbers = remaining_numbers


# 创建一个商品对象并测试
product666 = Product(666, "Iphone 15 Pro Max (1TB)", 13999, 100, 100)
product666.display()
print("已售出商品价值:", product666.income(10))
product666.display()
product666.setdata("Iphone 16 Pro Max (2TB)", 18888, 50, 50)
product666.display()
print("已售出商品价值:", product666.income(20))
product666.display()

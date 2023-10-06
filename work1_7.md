  class Product:
    # 初始化商品信息
    def _init_(self, product_number, product_name, unit_price, total_numbers, remaining_numbers):
        self.product_number = product_number
        self.product_name = product_name
        self.unit_price = unit_price
        self.total_numbers = total_numbers
        self.remaining_numbers = remaining_numbers

    # 显示商品信息
    def display(self):
        print(f商品序号: {self.product_number})
        print(f商品名: {self.product_name})
        print(f单价: {self.unit_price})
        print(f总数量: {self.total_numbers})
        print(f剩余数量: {self.remaining_numbers})

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


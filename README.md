# week-5# Parent class
class Device:
    def __init__(self, brand):
        self.brand = brand

    def power_on(self):
        print("Device is powering on...")


# Child class (Inheritance)
class Smartphone(Device):
    def __init__(self, brand, model, price):
        super().__init__(brand)   # call parent constructor
        self.model = model
        self.price = price

    def call(self):
        print(f"{self.model} is making a call 📞")

    def show_info(self):
        print(f"Brand: {self.brand}, Model: {self.model}, Price: ${self.price}")

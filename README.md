# discount-any-product-using-oops

class Laptop:
    #constructor
    def __init__(self,brand,model,price):
        self.brand = brand
        self.model = model
        self.price = price

    #method
    def discount_price(self,num):
        disc = self.price*(num/100)

        return f'After {num} % discount ammount will be',self.price - disc

#object
laptop1 = Laptop('HP','kfks',70000)
print(laptop1.price)
print(laptop1.discount_price(10))

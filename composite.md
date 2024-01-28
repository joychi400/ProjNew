use compsition to structure classobject
class  Animal:
	"""
	assign or embedd class objects as an instance
	"""

	def __init__(self):
		self.pet = Pet()  #embedd class object to instance attribute
		self.dog = Dog()
	def funcs(self):
		self.pet.func()
		self.dog.func()
class Cat:
	def func(self):
		print('meow')
class Dog:
	def func(self):
		print('wow wow!')

if __name__ == '__main__':
	animal = Animal()
	animal.funcs()
		
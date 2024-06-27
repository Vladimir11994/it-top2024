#            16.06.24          Аргументы по умолчаниюd
#def sum(a,b=3.14):
#    return a+b
#print(sum(4,5))
#                  Прмер
#def get_name(name='Иван'):
#    return  name
#print(get_name())
#print(get_name("Дмитрий"))
#                  Прмер
#class Car:
#    def __init__(self,speed,color='Yellow'):
#        self.speed=speed
#        self.colot=color
#car1 = Car(100)
#car2 = Car(100,'blue')
#print(f'{car1.color}')
#print(f'{car2.color}')
#                  Прмер
#class Car:
#    def __init__(self,speed,color='Yellow'):
#        self.speed=speed
#        self.colot=color
#        self.owner=owner
#def say_owne(self):
#    if self.owner:
#        print(f'Владелец{self.owner}')
#    else:
#        print('У данного автомобиля нет владельца')
#car1 =Car(100,'green','Иван')
#car2 =Car(90,'blue')
#print(f'{car1.color}')
#print(f'{car2.color}')
#                  Прмер
#class Car:
#    def __init__(self,speed,color='Yellow'):
#        self.speed=speed
 #       self.colot=color
#        self.owner=owner
#def say_owne(self):
#    if self.owner:
#        print(f'Владелец{self.owner}')
#    else:
#        print('У данного автомобиля нет владельца')
#car1 =Car(100,'green','Иван')
#car2 =Car(90,'blue')
#print(f'{car1.color}')
#print(f'{car2.color}')
#    Инкапсуляция              Прмер
#Инкапсуляция - это ограничение доступа состовляющим обьект компанентом
#(методы и переменными).Инкопсуляця делаяет некоторые из компанентов
#Доступ в нутри класса.
#
#                  Прмер
#class person:
#    _age=15
#person1=Person

#print(person1.age)
#person1._age=14
#print(person1._age)
#                  Прмер
#class person:
#    _age=15

#     def__say_hello(self):
#       print('Привет')
#person1= person
#print(person1._age)
# person1.__say_hello()
#                  Прмер
#class MyClasse:
#    def__init__(self,name):
#       self._name=name
#    @property
#    def name(self):
#        return self._name
#a = MyClass('Ivan')
#print(a.name)
#                  Прмер
#    Метод
#class Animal:
#    def __init__(self,name,breed='Без породы'):
#        self.name=name
#        self.breed=breed
#        def __say_breea(self):
#            print(self.bread)
#cat_Animal__say_breed('Барсик','Сибирский')
#cat._Animal__say_bred()
#dog = animal('Тузик')
#dog._Animal__say_breed()


#                              Домашняя работа 16.06.24 воскресенье
#         Задача№2
# Создаем множество из десяти вещей, которые бы взяли на необитаемый остров
#my_items = {"нож", "очки для солнца", "палатка", "компас", "зажигалка", "переносной фонарь", "палатка", "противомоскитная сетка", "переносное зарядное устройство", "книга"}

# Спрашиваем у близкого человека, какие вещи он бы взял на необитаемый остров
#their_items = {"нож", "очки для солнца", "палатка", "компас", "зажигалка", "переносной фонарь", "противомоскитная сетка", "переносное зарядное устройство", "книга", "еда"}

# Выводим на экран множество вещей, которые бы взяли оба
#both_items = my_items.intersection(their_items)
#print("Вещи, которые бы взяли оба:")
#print(both_items)

# Выводим на экран множество вещей, которые бы взял только я
#my_only_items = my_items.difference(their_items)
#print("\nВещи, которые бы взял я, но не мой близкий человек:")
#print(my_only_items)

#         Задача Дополнительная задача
#def remove_punctuation(input_string):
#    punctuation = '''!()-[]{};:'"\,<>./?@#$%^&*_~'''
#    output_string = ""
#    for char in input_string:
#    if char not in punctuation:
#    output_string += char
#    return output_string
#user_input = input("Введите строку: ")
#result = remove_punctuation(user_input)
#print("Результат после удаления знаков препинания:", result)

#                                         Домашняя работа за 19.06.24 число
#           Задача№1
#class Car:
#def __init__(self, make, model, year):
#self.make = make
#self.model = model
#self.year = year

#def display_info(self):
#print(f"Car: {self.year} {self.make} {self.model}")
#def __str__(self):
#return f"{self.year} {self.make} {self.model}"
#def __eq__(self, other):
#return self.make == other.make and self.model == other.model and self.year == other.year
# Пример использования
#car1 = Car("Toyota", "Corolla", 2020)
#car2 = Car("Toyota", "Corolla", 2020)

#car1.display_info()
#print(car1 == car2)
#           Задача№2

#class Book:
#def __init__(self, title, author, pages):
#self.title = title
#self.author = author
#self.pages = pages

#def __str__(self):
#return f"{self.title} by {self.author}"

#def __eq__(self, other):
#return self.title == other.title and self.author == other.author

#def __gt__(self, other):
#return self.pages > other.pages

# Пример использования
#book1 = Book("Python Programming", "John Smith", 300)
#book2 = Book("Java Basics", "Alice Johnson", 250)

#print(book1) # Вывод: Python Programming by John Smith
#print(book1 == book2) # Вывод: False
#print(book1 > book2) # Вывод: True
#                                        Задача№3
#class Stadium:
#def __init__(self, name, capacity, location):
#self.name = name
#self.capacity = capacity
#self.location = location
#def __str__(self):
#return f"Stadium: {self.name}, Capacity: {self.capacity}, Location: {self.location}"
#def __eq__(self, other):
#return self.name == other.name and self.capacity == other.capacity and self.location == other.location
#def __lt__(self, other):
#return self.capacity < other.capacity

# Пример использования:
#stadium1 = Stadium("Old Trafford", 75000, "Manchester")
#stadium2 = Stadium("Camp Nou", 99000, "Barcelona")

#print(stadium1)                                  С решением 3 задача подсказали если так понял .
#print(stadium2)

#if stadium1 == stadium2:
#print("The stadiums are the same.")
#else:
#print("The stadiums are different.")

#if stadium1 < stadium2:
#print(f"{stadium1.name} has a smaller capacity than {stadium2.name}.")
#else:
#print(f"{stadium2.name} has a smaller capacity than {stadium1.name}.")

#                                 Домащняя работа 12.06.24
#             Задача №1
#class Car:
#  def __init__(self, model_name=None, year=None, manufacturer=None, engine_volume=None, color=None, price=None):
#       self.model_name = model_name
#       self.year = year
#       self.manufacturer = manufacturer
#       self.engine_volume = engine_volume
#       self.color = color
#       self.price = price
# def set_model_name(self, model_name):
#        self.model_name = model_name
#    def set_year(self, year):
#        self.year = year
#    def set_manufacturer(self, manufacturer):
#        self.manufacturer = manufacturer
#    def set_engine_volume(self, engine_volume):
#        self.engine_volume = engine_volume
#    def set_color(self, color):
#         self.color = color
#    def set_price(self, price):
#         self.price = price
#    def get_model_name(self):
#         return self.model_name
#    def get_year(self):
#         return self.year
#    def get_manufacturer(self):
#         return self.manufacturer
#    def get_engine_volume(self):
#         return self.engine_volume
#    def get_color(self):
#         return self.color
#    def get_price(self):
#         return self.price
#    def display_car_info(self):
#       print("Model name:", self.model_name)
#       print("Year:", self.year
#       print("Manufacturer:", self.manufacturer)
 #      print("Engine volume:", self.engine_volume)
 #      print("Color:", self.color)
 #      print("Price:", self.price)
#   def input_car_info(self):
#       self.set_model_name(input("Enter model name: "))
#      self.set_year(input("Enter year of production: "))
#       self.set_manufacturer(input("Enter manufacturer: "))
#       self.set_engine_volume(input("Enter engine volume: "))
#        self.set_color(input("Enter color: "))
#        self.set_price(input("Enter price: ")
#             Задача №2
#class Book:
#    def __init__(self, book_name=None, year=None, publisher=None, genre=None, author=None, price=None):
#      self.book_name = book_name
#      self.year = year
#      self.publisher = publisher
#      self.genre = genre
#      self.author = author
#      self.price = price
#    def set_book_name(self, book_name):
#      self.book_name = book_name
#    def set_year(self, year):
#      self.year = year
#    def set_publisher(self, publisher):
#      self.publisher = publisher
#    def set_genre(self, genre):
#      self.genre = genre
#    def set_author(self, author):
#      self.author = author
#    def set_price(self, price):
#      self.price = price
 ##  def get_book_name(self):
#     return self.book_name
#   def get_year(self):
#     return self.year
#   def get_publisher(self):
#     return self.publisher
#   def get_genre(self):
#     return self.genre
#   def get_author(self):
#      return self.author
#   def get_price(self):
#       return self.price
#   def display_book_info(self):
#       print("Book name:", self.book_name)
#       print("Year:", self.year)
#       print("Publisher:", self.publisher)
 #      print("Genre:", self.genre)
#       print("Author:", self.author)
#       print("Price:", self.price)
 #  def input_book_info(self):
#       self.set_book_name(input("Enter book name: "))
#       self.set_year(input("Enter year of publication: "))
#       self.set_publisher(input("Enter publisher: "))
#       self.set_genre(input("Enter genre: "))
#       self.set_author(input("Enter author: "))
#       self.set_price(input("Enter price: "))
#                                     23.06.24. Воскресенье Д.з
#               Задача№1
#class Person:
#pass

#id_1 = Person()

#setattr(id_1, "name", "Vasya")
#setattr(id_1, "name", "Masha")

#print(id_1.name)
#               Задача№2
#class Person:
#setup = ['set_name', 'set_age', 'set_work', 'set_study']

#id_1 = Person()

#for attr in id_1.setup:
#value = input(f"Введите значение для атрибута {attr}: ")
#setattr(id_1, attr, value)
#               Задача№3
#class Person:
#def __init__(self):
#self.dance = "salsa"
#self.music = "rock"
#self.age = 30

#id_1 = Person()
# Используем цикл for
#attributes = ['dance', 'music', 'age']
#for attr in attributes:
#print(getattr(id_1, attr))
# Или без цикла
#print(getattr(id_1, 'dance'))
#print(getattr(id_1, 'music'))
#print(getattr(id_1, 'age'))
#                                     26.06.24. Воскресенье Д.з
#            Задача№1
#class Homer:
#    def __init__(self, name):
#     self.name = name

#class Daughter(Homer):
#    pass

#daughter1 = Daughter("Lisa")
#print(daughter1.name)
#            Задача№2
#class Shape:
#    def calculate_area(self):
#    pass
#class Rectangle(Shape):
#    def __init__(self, width, height):
#self.width = width
#self.height = height

#    def calculate_area(self):
#return self.width * self.height

#class Circle(Shape):
#    def __init__(self, radius):
#self.radius = radius

#    def calculate_area(self):
#return 3.14 * self.radius * self.radius

#class Triangle(Shape):
#    def __init__(self, base, height):
#self.base = base
#self.height = height

#    def calculate_area(self):
#return 0.5 * self.base * self.height

#rectangle = Rectangle(5, 10)
#print("Площадь прямоугольника:", rectangle.calculate_area())

#circle = Circle(7)
#print("Площадь круга:", circle.calculate_area())

#triangle = Triangle(4, 6)
#print("Площадь треугольника:", triangle.calculate_area())
#            Задача№3
#class Animal:
#    def make_sound(self):
#    pass
#class Dog(Animal):
#    def make_sound(self):
#print("Woof")

#class Cat(Animal):
#    def make_sound(self):
#print("Meow")
#class Bird(Animal):
#    def make_sound(self):
#print("Tweet")






















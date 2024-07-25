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

#                                  30.07.24 Воскересенье Дз
#            Задача№1

#class Bank:
 #   def __init__(self, client_name, card_number, initial_balance):
 #         self.__client_name = client_name
 #         self.__card_number = card_number
#          self.__balance = initial_balance

 #   def print_balance(self):
#print(f"Client: {self.__client_name}, Card Number: {self.__card_number}, Balance: {self.__balance}")

#    def change_balance(self, money):
#    if money < 0:
#print("Withdrawal operation")
#    self.__balance += money
#    elif money > 0:
#print("Deposit operation")
#    self.__balance += money
#    else:
#print("No changes made to the balance")
# Пример использования класса Bank
#client1 = Bank("Alice", "1234 5678 9012 3456", 1000)
#client1.print_balance()

#client1.change_balance(500)
#client1.print_balance()

#client1.change_balance(-200)
#client1.print_balance()
#                        Задание: №2
#class Account:
#    def __init__(self, balance):
#          self.__balance = balance

#@property
#    def balance(self):
#    return self.__balance

#@balance.setter
#    def balance(self, new_balance):
#    self.__balance = new_balance

#@balance.deleter
#    def balance(self):
#    self.__balance = 0

# Проверка кода
#acc = Account(100)
#print(acc.balance) # Вывод: 100
#acc.balance = 200
#print(acc.balance) # Вывод: 200
#del acc.balance
#print(acc.balance) # Вывод: 0

#                              03.07.24 среда Домашняя работа
#    Задача №1
#import math

#_default_radius = 5

#   def circle_perimeter(radius=_default_radius):
#   return 2 * math.pi * radius

#   def circle_area(radius=_default_radius):
#   return math.pi * radius**2
#from circle import circle_perimeter, circle_area
#print(circle_perimeter(3)) # Выведет длину окружности с радиусом 3
#print(circle_area(3)) # Выведет площадь окружности с радиусом 3
#    Задача №2
#def triangle_perimeter(a=7, b=2, c=8):
#perimeter = a + b + c
#return perimeter

#def triangle_area(a=7, b=2, c=8):
#s = (a + b + c) / 2
#area = (s * (s - a) * (s - b) * (s - c)) ** 0.5
#return area
# triangle.py
#a = 7
#b = 2
#c = 8

#def triangle_perimeter(side_a=None, side_b=None, side_c=None):
#a_side = a if side_a is None else side_a
#b_side = b if side_b is None else side_b
#c_side = c if side_c is None else side_c

#perimeter = a_side + b_side + c_side
#return perimeter

#def triangle_area(side_a=None, side_b=None, side_c=None):
#a_side = a if side_a is None else side_a
#b_side = b if side_b is None else side_b
#c_side = c if side_c is None else side_c
#s = (a_side + b_side + c_side) / 2
#area = (s * (s - a_side) * (s - b_side) * (s - c_side)) ** 0.5
#return area
#    Задача №3
#def square_perimeter(a=15):
#return 4 * a

#def square_area(a=15):
#return a * a
#import square

#perimeter = square.square_perimeter() # Периметр квадрата со стороной 15
#area = square.square_area() # Площадь квадрата со стороной 15

#print("Периметр квадрата:", perimeter)
#print("Площадь квадрата:", area)
#   Игра мяу-кэт
#import pygame, sys
#pygame.init()
#screen = pygame.display.set_mode((500, 500))
#clock = pygame.time.Clock()
#while True:
 #  for event in pygame.event.get():
 #      if event.type == pygame.QUIT:
 #          pygame.quit()
#           sys.exit()
#   screen.fill((30, 30, 30))
#   pygame.display.update()
#   clock.tick(120)
#class ParticlePrinciple:
#   def __init__(self):
#       self.particles = []

#   def emit(self):
#       pass
#   def add_particles(self):
 #      pass
#   def delete_particles(self):
#       pass
#PARTICLE_EVENT = pygame.USEREVENT + 1
#pygame.time.set_timer(PARTICLE_EVENT, 40)
#   pass
#particle1 = ParticlePrinciple()
#def add_particles(self):
#   pos_x = 250
#   pos_y = 250
#   radius = 10
#direction = -1
#particle_circle = [[pos_x, pos_y], radius, direction]
#self.particles.append(particle_circle)
#def emit(self):
#   if self.particles:
#       for particle in self.particles:
#           pass
#def emit(self):
#   if self.particles:
#       for particle in self.particles:
#           particle[0][1] += particle[2]
#           particle[1] -= 0.2
#           pygame.draw.circle(screen, pygame.Color('White'), particle[0], int(particle[1]))
#screen.fill((30, 30, 30))
#particle1.emit()
#def delete_particles(self):
 #  particles_copy = [particle for particle in self.particles if particle[1] > 0]
#   self.particles = particles_copy
#    if self.particles:
#        self.delete_particles()
#        for particle in self.particles:
#            particle[0][1] += particle[2]
#            particle[1] -= 0.2
#            pygame.draw.circle(screen, pygame.Color('White'), particle[0], int(particle[1]))
#direction = -3
#nyan_surface = pygame.image.load('images/nyan_cat.png').convert_alpha()
#pygame.time.set_timer(PARTICLE_EVENT, 150)
#pos_x = pygame.mouse.get_pos()[0]
#pos_y = pygame.mouse.get_pos()[1]
#direction = random.randint(-3, 3)#
#particle[0][0] += particle[2]
#direction_x = random.randint(-3, 3)
#direction_y = random.randint(-3, 3)
#particle_circle = [[pos_x, pos_y], radius, [direction_x, direction_y]]
#def emit(self):
#   if self.particles:
#       self.delete_particles()
#       for particle in self.particles:
#           particle[0][1] += particle[2][0]
 #          particle[0][0] += particle[2][1]
#           particle[1] -= 0.2
#           pygame.draw.circle(screen, pygame.Color('White'), particle[0], int(particle[1]))
#class ParticlePrinciple:
#   def __init__(self):
#       self.particles = []
#       self.size = 8
#def add_particles(self, offset, color):
#   pos_x = pygame.mouse.get_pos()[0]
#   pos_y = pygame.mouse.get_pos()[1] + offset
#   particle_rect = pygame.Rect(pos_x - self.size / 2, pos_y - self.size / 2,self.size, self.size)
#   self.particles.append((particle_rect, color))
#def emit(self):
#   if self.particles:
#       self.delete_particles()
#       for particle in self.particles:
#           particle[0].x -= 2
#if event.type == PARTICLE_EVENT:
   # particle1.add_particles()
#   particle2.add_particles(0, pygame.Color('Green'))
# particle1.emit()
#particle2.emit()
#def delete_particles(self):
#   particles_copy = [particle for particle in self.particles if particle[0].x > 0]
#   self.particles = particles_copy
#particle2.add_particles(-20, pygame.Color('Pink'))
#particle2.add_particles(-12, pygame.Color('Gray'))
#particle2.add_particles(-4, pygame.Color('Cold'))
#particle2.add_particles(4, pygame.Color('Silver'))
#particle2.add_particles(12, pygame.Color('indigo'))
#particle2.add_particles(20, pygame.Color('violet'))
#pygame.time.set_timer(PARTICLE_EVENT, 40)
#def emit(self):
# if self.particles:
#       self.delete_particles()
#       for particle in self.particles:
#           particle[0].x -= 1
#                                          Домашняя работа      10.07.24
#               Задача1
#def flatten(lst, depth):
#  result = []
#for item in lst:
# if isinstance(item, list) and depth > 0:
#  result.extend(flatten(item, depth - 1))
#else:
# result.append(item)
# return result
# Пример использования функции
#nested_list = [1, [2, [3, 4], 5], 6, [7, 8]]
#depth = 2
#flattened_list = flatten(nested_list, depth)
#print(flattened_list)
#               Задача2
#def unpack_list(nested_list):
# flat_list = []
#for item in nested_list:
# if isinstance(item, list):
#  flat_list.extend(unpack_list(item))
#else:
# flat_list.append(item)
#return flat_list
# Пример использования функции
#nested_list = [1, [2, 3], [4, [5, 6]], 7]
#result = unpack_list(nested_list)
#print(result)


#                                                 Домашняя работа     15.07.24
#                                        Задача№1
#def flatten(lst, depth):
# result = []
#for item in lst:
# if isinstance(item, list) and depth > 0:
#  result.extend(flatten(item, depth - 1))
#else:
# result.append(item)
#return result
#nested_list = [1, [2, [3, 4], 5], 6, [7, 8]]
#depth = 2
#flattened_list = flatten(nested_list, depth)
#print(flattened_list)
#                                          Задача№2
#def flatten_list(nested_list):
#for item in nested_list:
#  flat_list.extend(flatten_list(item))
#else:
# flat_list.append(item)
#return flat_list
#nested_list = [1, [2, 3], [4, [5, 6]], 7]
#flattened_list = flatten_list(nested_list)
#print(flattened_list)
#                                          Задача№3
     # С ДАННОЙ ЗАДАЧЕЙ ПОДСКАЗАЛИ
#def unpack_lists(input_list):
# output_list = []
#for item in input_list:
# if isinstance(item, list):
#  output_list.extend(unpack_lists(item))
#else:
# output_list.append(item)
#return output_list
#nested_list = [[1, 2], [3, [4, 5]], 6, [7, 8, [9, 10]]]
#result = unpack_lists(nested_list)
#print(result)

#                                             Домашняя работа 17.07.24
#                  Задача№1
#def log_errors(func):
# """ Декоратор логирования ошибок """
# def decorator(a, b, oper):
 # try:
#   return func(a, b, oper)
#  except:
#   msg = 'Функция {} выдала ошибку с параметрами: a={}, b={}, oper={}'.format(func.__name__, a, b, oper)
#   print(msg)
#  return None
# return decorator
#@log_errors
#def calculate(a: int, b: int, oper: str):
 #""" Функция выполнения арифметической операции между двумя числами """
# expression = '{} {} {}'.format(a, oper, b)
# res = eval(expression)
# return res
#r = calculate(1, 2, '+')
#print(r)
#print(r)
#return func(a, b, oper)
#except Exception as e:
#print(f"An error occurred: {e}")
#return decorator
#@log_errors
#def calculate(a, b, oper):
#if oper == '+':
#return a + b
#elif oper == '-':
#return a - b
#elif oper == '*':
#return a * b
#elif oper == '/':
#return a / b
# Пример использования
#result = calculate(10, 5, '+')
#print(result)

#                                      Домашняя работа 21.07.24
#                   Задача№1
#def role_required(role: str):
#def decorator(func):
#def wrapper(user_role):
#if user_role == 'admin':
#return func()
#else:
#return 'Permission denied'
#return wrapper
#return decorator
#@role_required('admin')
#def secret_resource():
#return 'Permission accepted'
# Пример использования
#user_role = input().strip()
#result = secret_resource(user_role)
#print(result)

#                               24.07.24 Среда занятие класс
#      Тема
#  Фабричный метод
#     Значения метода фабричный
#Фабричный метод это пораждаюши  фактор
#проектирования который определеяет обший интер фейс
#для создания обьектов супер-классов позволяет подклассам
#изменять тип создоваемых обьектов
#   Пример
#class Documet(object):
#    def show(self):
#        raise  NotImplementedError()

#class ODFDocument(Documet):
#     def show(self):
#         print('Открытие формата документа')

#class MSOficeDocument(Documet):
#     def show(self):
#         print('MSOffice формат')

#class Application(object):
#     def create_document(self,type_):
#         raise NotImplementedError

#class MyApplication(Application):
#     def create_document(self,type_):
#         if type_=='odf':
#             return ODFDocument()
#         elif type_=='doc':
#             return  MSOficeDocument()
#         else:
#             return  Documet()

#app = MyApplication()
#app.create_document('odf').show()
#app.create_document('doc').show()

#try:
#    app.create_document('pdf').show()
#except:
#      print('NotImplementedError')
#           ПРОТОТИП дальше тема
#прототип создает виды создаваемых обьектов с помощью
#экземпляра прототипа.
#                        Пример
#import copy
#from typing import Dict, Any
#class Prototype:
#    def _init_(self) -> None:
#        self._objects: Dict[str, Any] = {}

 #   def register(self, name: str, obj: Any) -> None:
 #       self._objects[name] = obj

#    def unregister(self, name: str) -> None:
#        del self._objects[name]

#    def clone(self, name: str, attrs: Dict[str, Any]) -> Any:
#        obj = copy.deepcopy(self._objects[name])
#        obj._dict_.update(attrs)
#        return obj
#class Bird:
#    """Птица"""

#    def _init_(self, name: str = "") -> None:
#        self.name = name

    # Создаем экземпляр прототипа
#prototype = Prototype()
#prototype.register('bird', Bird())
# Клонируем и изменяем атрибуты для совы
#owl = prototype.clone('bird', {'name': 'Owl'})
#print(type(owl), owl.name)  # <class '_main_.Bird'> Owl
# Клонируем и изменяем атрибуты для утки
#duck = prototype.clone('bird', {'name': 'Duck'})
#print(type(duck), duck.name)  # <class '_main_.Bird'> Duck
#             Пример
#class WindowsBase(object):
#    def show(self):
#        raise  NotImplementedError()
#    def hide(self):
#         raise NotImplementedError()

#class MainWindow(WindowsBase):
 #    def show(self):
 #     raise  NotImplementedError()
 #    print('Показать MainWindow')
     #     def hide(self):
#         print('Спрятать MainWindow')

#class SettingWindows(WindowsBase):
# def hide(self):
#  print('Спрятать MainWindow')

#def hide(self):
# print('Спрятать SettingWindow')

#class WindowMediator(object):
#     def __init__(self):
#         self.windows=dict.fromkeys(['main','setting','help'])

#     def show(self,win):
#          for window in self.windows.values():
#              if not window is win:
#                  window.hide()
#             Пример
#                                      24.05.24   Домашняя  работа
#                 Задача№1
#def role_required(role: str):
#def decorator(func):
#def wrapper(user_role):
#if user_role == 'admin':
#return func()
#else:
#return 'Permission denied'
#return wrapper
#return decorator

#@role_required('admin')
#def secret_resource():
#return 'Permission accepted'
# Пример использования
#print(secret_resource('admin')) # Output: Permission accepted
#print(secret_resource('manager')) # Output: Permission denied
#                 Задача№2
#RU_TO_EN = {
#"привет": "hello",
#"мир": "world"
#}
#RU_TO_LT = {
#"привет": "sveiki",
#"мир": "pasaulis"
#}
#def translate_to(lang: str):
#def decorator(func):
#def wrapper(word):
#if lang == "EN":
#translation = RU_TO_EN.get(word, word)
#elif lang == "LT":
#translation = RU_TO_LT.get(word, word)
#else:
#translation = word
#return func(translation)
#return wrapper
#return decorator

#@translate_to("EN")
#def say(word):
#print(word)

#@translate_to("LT")
#def say_lt(word):
#print(word)
#say("привет")
#say_lt("привет")











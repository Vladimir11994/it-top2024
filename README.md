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

 #       переписать 10 паттернов
# coding: utf-8
#              Паттерны №1
"""
Абстрактная фабрика (Abstract factory, Kit) - паттерн, порождающий объекты.

#Предоставляет интерфейс для создания семейств взаимосвязанных или взаимозависимых объектов,
#не специфицируя их конкретных классов.

#Классы абстрактной фабрики часто реализуются фабричными методами,
#но могут быть реализованы и с помощью паттерна прототип.
#"""
#class AbstractFactory(object):
#    def create_drink(self):
#        raise NotImplementedError()

#    def create_food(self):
#        raise NotImplementedError()
#class Drink(object):
#    def __init__(self, name):
#        self._name = name

#    def __str__(self):
#        return self._name
#class Food(object):
#    def __init__(self, name):
#        self._name = name

#    def __str__(self):
#        return self._name

#class ConcreteFactory1(AbstractFactory):
#    def create_drink(self):
#        return Drink('Coca-cola')

#    def create_food(self):
#        return Food('Hamburger')
#class ConcreteFactory2(AbstractFactory):
#    def create_drink(self):
#        return Drink('Pepsi')

#    def create_food(self):
#        return Food('Cheeseburger')
#def get_factory(ident):
#    if ident == 0:
#        return ConcreteFactory1()
#    elif ident == 1:
#        return ConcreteFactory2()

#factory = get_factory(1)
#print factory.create_drink()  # Pepsi
#print factory.create_food()  # Cheeseburger
#              Паттерны №2
# coding: utf-8

"""
Строитель (Builder) - паттерн, порождающий объекты.

Отделяет конструирование сложного объекта от его представления,
так что в результате одного и того же процесса конструирования могут получаться разные представления.

От абстрактной фабрики отличается тем, что делает акцент на пошаговом конструировании объекта.
Строитель возвращает объект на последнем шаге, тогда как абстрактная фабрика возвращает объект немедленно.

Строитель часто используется для создания паттерна компоновщик.
"""
#class Builder(object):
#    def build_body(self):
#        raise NotImplementedError()
#    def build_lamp(self):
#        raise NotImplementedError()

#    def build_battery(self):
#        raise NotImplementedError()

#    def create_flashlight(self):
#        raise NotImplementedError()
#class Flashlight(object):
#    """Карманный фонарик"""
#    def __init__(self, body, lamp, battery):
#        self._shine = False  # излучать свет
#        self._body = body
#        self._lamp = lamp
#        self._battery = battery
#    def on(self):
#        self._shine = True
#    def off(self):
#        self._shine = False
#    def __str__(self):
#        shine = 'on' if self._shine else 'off'
#        return 'Flashlight [%s]' % shine
#class Lamp(object):
#    """Лампочка"""
#class Body(object):
#    """Корпус"""
#class Battery(object):
#    """Батарея"""
#class FlashlightBuilder(Builder):
#    def build_body(self):
#        return Body()
#    def build_battery(self):
#        return Battery()
#    def build_lamp(self):
#        return Lamp()
#    def create_flashlight(self):
#        body = self.build_body()
#        lamp = self.build_lamp()
#        battery = self.build_battery()
#        return Flashlight(body, lamp, battery)
#builder = FlashlightBuilder()
#flashlight = builder.create_flashlight()
#flashlight.on()
#print flashlight  # Flashlight [on]
#              Паттерны №3
# coding: utf-8

"""
Фабричный метод (Factory Method) - паттерн, порождающий классы.

Определяет интерфейс для создания объекта, но оставляет подклассам решение о том, какой класс инстанцировать.
Позволяет делегировать инстанцирование подклассам.

Абстрактная фабрика часто реализуется с помощью фабричных методов.
Фабричные методы часто вызываются внутри шаблонных методов.
"""
#class Document(object):
#    def show(self):
#        raise NotImplementedError()
#class ODFDocument(Document):
#    def show(self):
#        print 'Open document format'
#class MSOfficeDocument(Document):
#    def show(self):
#        print 'MS Office document format'
#class Application(object):
#    def create_document(self, type_):
        # параметризованный фабричный метод `create_document`
#        raise NotImplementedError()
#class MyApplication(Application):
#    def create_document(self, type_):
#        if type_ == 'odf':
#            return ODFDocument()
#        elif type_ == 'doc':
 #           return MSOfficeDocument()
#        else:
#            return Document()
#app = MyApplication()
#app.create_document('odf').show()  # Open document format
#app.create_document('doc').show()  # MS Office document format
#try:
#    app.create_document('pdf').show()
#except:
#    print("NotImplementedError")
#              Паттерны №4
# coding: utf-8

"""
Прототип - паттерн, порождающий объекты.
Задает виды создаваемых объектов с помощью экземпляра-прототипа
#и создает новые объекты путем копирования этого прототипа.
#"""
#import copy
#class Prototype(object):
#    def __init__(self):
#        self._objects = {}

#    def register(self, name, obj):
#        self._objects[name] = obj

#    def unregister(self, name):
#        del self._objects[name]
#    def clone(self, name, attrs):
#        obj = copy.deepcopy(self._objects[name])
#        obj.__dict__.update(attrs)
#        return obj
#class Bird(object):
#    """Птица"""
#prototype = Prototype()
#prototype.register('bird', Bird())
#owl = prototype.clone('bird', {'name': 'Owl'})
#print type(owl), owl.name  # <class '__main__.Bird'> Owl
#duck = prototype.clone('bird', {'name': 'Duck'})
#print type(duck), duck.name  # <class '__main__.Bird'> Duck
#              Паттерны №5
# coding: utf-8

"""
Одиночка (Singleton) - паттерн, порождающий объекты.

Гарантирует, что у класса есть только один экземпляр, и предоставляет к нему глобальную точку доступа.

С помощью паттерна одиночка могут быть реализованы многие паттерны (абстрактная фабрика, строитель, прототип).
"""
#class SingletonMeta(type):
#    def __init__(cls, *args, **kwargs):
#        cls._instance = None
#        # глобальная точка доступа `Singleton.get_instance()`
#        cls.get_instance = classmethod(lambda c: c._instance)
#        super(SingletonMeta, cls).__init__(*args, **kwargs)
#    def __call__(cls, *args, **kwargs):
#        if not cls._instance:
#            cls._instance = super(SingletonMeta, cls).__call__(*args, **kwargs)
#        return cls._instance
#class Singleton(object):
#    __metaclass__ = SingletonMeta
#    def __init__(self, name):
#        self._name = name
#    def get_name(self):
#        return self._name
#obj1 = Singleton('MyInstance 1')
#print obj1.get_name()  # MyInstance 1
#obj2 = Singleton('MyInstance 2')
#print obj2.get_name()  # MyInstance 1
#print obj1 is obj2 is Singleton.get_instance()  # True
#              Паттерны №6
# coding: utf-8

"""
Цепочка обязанностей (Chain of Responsibility) - паттерн поведения объектов.

Позволяет избежать привязки отправителя запроса к его получателю,
давая шанс обработать запрос нескольким объектам. Связывает объекты-получатели в цепочку
и передает запрос вдоль этой цепочки, пока его не обработают.
"""
#class HttpHandler(object):
#    """Абстрактный класс обработчика"""
#    def handle(self, code):
#        raise NotImplementedError()
#class Http404Handler(HttpHandler):
#    """Обработчик для кода 404"""
#    def handle(self, code):
#        if code == 404:
#            return 'Страница не найдена'
#class Http500Handler(HttpHandler):
#    """Обработчик для кода 500"""
#    def handle(self, code):
#        if code == 500:
#            return 'Ошибка сервера'
#class Client(object):
 #   def __init__(self):
#        self._handlers = []
#    def add_handler(self, h):
#        self._handlers.append(h)
#    def response(self, code):
#        for h in self._handlers:
#            msg = h.handle(code)
#            if msg:
#                print 'Ответ: %s' % msg
#                break
 #       else:
#            print 'Код не обработан'
#client = Client()
#client.add_handler(Http404Handler())
#client.add_handler(Http500Handler())
#client.response(400)  # Код не обработан
#client.response(404)  # Ответ: Страница не найдена
#client.response(500)  # Ответ: Ошибка сервера
#              Паттерны №7
# coding: utf-8

"""
Команда (Command, Action, Transaction) - паттерн поведения объектов.

Инкапсулирует запрос как объект, позволяя тем самым задавать параметры клиентов
для обработки соответствующих запросов, ставить запросы в очередь или протоколировать их,
а также поддерживать отмену операций.
"""
#class Light(object):
#    def turn_on(self):
#        print 'Включить свет'
#    def turn_off(self):
#        print 'Выключить свет'
#class CommandBase(object):
#    def execute(self):
#        raise NotImplementedError()
#class LightCommandBase(CommandBase):
 #   def __init__(self, light):
#        self.light = light
#class TurnOnLightCommand(LightCommandBase):
#    def execute(self):
#        self.light.turn_on()
#class TurnOffLightCommand(LightCommandBase):
#    def execute(self):
#        self.light.turn_off()
#class Switch(object):
#    def __init__(self, on_cmd, off_cmd):
#        self.on_cmd = on_cmd
#        self.off_cmd = off_cmd
#    def on(self):
#        self.on_cmd.execute()
#    def off(self):
#        self.off_cmd.execute()
#light = Light()
#switch = Switch(on_cmd=TurnOnLightCommand(light),
#                off_cmd=TurnOffLightCommand(light))
#switch.on()  # Включить свет
#switch.off()  # Выключить свет
#              Паттерны №8
# coding: utf-8

"""
Итератор (Iterator) - паттерн поведения объектов.

Предоставляет способ последовательного доступа ко всем элементам составного объекта,
не раскрывая его внутреннего представления.
"""
#class IteratorBase(object):
#    """Базовый класс итератора"""
#    def first(self):
#        """Возвращает первый элемент коллекции.
#        Если элемента не существует возбуждается исключение IndexError."""
#        raise NotImplementedError()
#    def last(self):
 #       """Возвращает последний элемент коллекции.
#        Если элемента не существует возбуждается исключение IndexError."""
#        raise NotImplementedError()
#    def next(self):
#        """Возвращает следующий элемент коллекции"""
#        raise NotImplementedError()
#    def prev(self):
#        raise NotImplementedError()
#    def current_item(self):
#        """Возвращает текущий элемент коллекции"""
#        raise NotImplementedError()
#    def is_done(self, index):
#        """Возвращает истину если элемент с указанным индексом существует, иначе ложь"""
#        raise NotImplementedError()
#    def get_item(self, index):
#        """Возвращает элемент коллекции с указанным индексом, иначе возбуждает исключение IndexError"""
#        raise NotImplementedError()
#class Iterator(IteratorBase):
#    def __init__(self, list_=None):
#        self._list = list_ or []
#        self._current = 0
 #   def first(self):
#        return self._list[0]
#    def last(self):
#        return self._list[-1]
#    def current_item(self):
#        return self._list[self._current]
#    def is_done(self, index):
#        last_index = len(self._list) - 1
#        return 0 <= index <= last_index#
#    def next(self):
#        self._current += 1
#        if not self.is_done(self._current):
#            self._current = 0
#        return self.current_item()
#    def prev(self):
#        self._current -= 1
#        if not self.is_done(self._current):
#            self._current = len(self._list) - 1
#        return self.current_item()
#    def get_item(self, index):
 #       if not self.is_done(index):
#            raise IndexError('Нет элемента с индексом: %d' % index)
#        return self._list[index]
#it = Iterator(['one', 'two', 'three', 'four', 'five'])
#print [it.prev() for i in range(5)]  # ['five', 'four', 'three', 'two', 'one']
#print [it.next() for i in range(5)]  # ['two', 'three', 'four', 'five', 'one']
#              Паттерны №9
# coding: utf-8

"""
Посредник (Mediator) - паттерн поведения объектов.

Определяет объект, инкапсулирующий способ взаимодействия множества объектов.
Посредник обеспечивает слабую связанность системы, избавляя объекты от необъодимости явно ссылаться друг на друга
и позволяя тем самым независимо изменять взаимодействия между ними.
"""
#class WindowBase(object):
#    def show(self):
#        raise NotImplementedError()
#    def hide(self):
#        raise NotImplementedError()
#class MainWindow(WindowBase):
#    def show(self):
#        print 'Show MainWindow'
#    def hide(self):
#        print 'Hide MainWindow'
#class SettingWindow(WindowBase):
#        print 'Show SettingWindow'
#    def hide(self):
#        print 'Hide SettingWindow'
#class HelpWindow(WindowBase):
#    def show(self):
#        print 'Show HelpWindow'
#    def hide(self):
#        print 'Hide HelpWindow'
#class WindowMediator(object):
#    def __init__(self):
#        self.windows = dict.fromkeys(['main', 'setting', 'help'])

#    def show(self, win):
#        for window in self.windows.itervalues():
#            if not window is win:
#                window.hide()
#        win.show()
#    def set_main(self, win):
#        self.windows['main'] = win
#    def set_setting(self, win):
#        self.windows['setting'] = win
#    def set_help(self, win):
#        self.windows['help'] = win
#main_win = MainWindow()
#setting_win = SettingWindow()
#help_win = HelpWindow()
#med = WindowMediator()
#med.set_main(main_win)
#med.set_setting(setting_win)
#med.set_help(help_win)
#main_win.show()  # Show MainWindow
#med.show(setting_win)
# Hide MainWindow
# Hide HelpWindow
# Show SettingWindow
#med.show(help_win)
# Hide MainWindow
# Hide SettingWindow
# Show HelpWindow
#              Паттерны №10
# coding: utf-8

"""
Состояние (State) - паттерн поведения объектов.

Позволяет объекту варьировать свое поведение в зависимости от внутреннего состояния.
Извне создается впечатление, что изменился класс объекта.
"""
#class LampStateBase(object):
#    """Состояние лампы"""
#    def get_color(self):
#        raise NotImplementedError()
#class GreenLampState(LampStateBase):
#    def get_color(self):
#        return 'Green'
#class RedLampState(LampStateBase):
#    def get_color(self):
#        return 'Red'
#class BlueLampState(LampStateBase):
#    def get_color(self):
#        return 'Blue'
#class Lamp(object):
#    def __init__(self):
#        self._current_state = None
#        self._states = self.get_states()
#    def get_states(self):
#        return [GreenLampState(), RedLampState(), BlueLampState()]
#    def next_state(self):
#        if self._current_state is None:
#            self._current_state = self._states[0]
#        else:
#            index = self._states.index(self._current_state)
#            if index < len(self._states) - 1:
#                index += 1
#            else:
#                index = 0
#            self._current_state = self._states[index]
#        return self._current_state
#    def light(self):
#        state = self.next_state()
#        print state.get_color()
#lamp = Lamp()
#[lamp.light() for i in range(3)]
# Green
# Red
# Blue
#[lamp.light() for i in range(3)]
# Green
# Red
# Blue
#                                28.07.24 Домашняя работа
#           Задач№1
#class Singleton:
# _instance = None
# def __new__(cls):
#  if cls._instance is None:
#  cls._instance = super(Singleton, cls).__new__(cls)
# return cls._instance
# Пример использования
#singleton1 = Singleton()
#singleton2 = Singleton()
#print(singleton1 is singleton2)  # Выведет True, так как singleton1 и singleton2 указывают на один и тот же объект
#singleton1 = Singleton()
#singleton2 = Singleton()

#print(singleton1 is singleton2)
#           Задач№2
#class AbstractFactory:
 #def create_product_a(self):
#  pass
#def create_product_b(self):
# pass
# Конкретная фабрика 1
#class ConcreteFactory1(AbstractFactory):
# def create_product_a(self):
#  return ConcreteProductA1()
# return ConcreteProductB1()
# Конкретная фабрика 2
#class ConcreteFactory2(AbstractFactory):
# def create_product_a(self):
#  return ConcreteProductA2()
#def create_product_b(self):
# return ConcreteProductB2()
# Абстрактный продукт A
#class AbstractProductA:
 #def operation(self):
 # pass
# Абстрактный продукт B
#class AbstractProductB:
 #def operation(self):
#  pass
# Конкретный продукт A1
#class ConcreteProductA1(AbstractProductA):
# def operation(self):
#  return "ConcreteProductA1 operation"
# Конкретный продукт B1
#class ConcreteProductB1(AbstractProductB):
# def operation(self):
#  return "ConcreteProductB1 operation"
# Конкретный продукт A2
#class ConcreteProductA2(AbstractProductA):
# def operation(self):
#  return "ConcreteProductA2 operation"
# Конкретный продукт B2
#class ConcreteProductB2(AbstractProductB):
# def operation(self):
#  return "ConcreteProductB2 operation"
# Тестирование
#factory1 = ConcreteFactory1()
#product_a1 = factory1.create_product_a()
#product_b1 = factory1.create_product_b()
#print(product_a1.operation())  # Вывод: ConcreteProductA1 operation
#print(product_b1.operation())  # Вывод: ConcreteProductB1 operation
#factory2 = ConcreteFactory2()
#product_a2 = factory2.create_product_a()
#product_b2 = factory2.create_product_b()
#print(product_a2.operation())  # Вывод: ConcreteProductA2 operation
#print(product_b2.operation())  # Вывод: ConcreteProductB2 operation
#                             Домашняя работа 31.07.24 Среда
#     Переписать код
#my_items = [
#    {'name': 'bread', 'price': 0.5, 'quantity': 20},
#    {'name': 'milk', 'price': 1.0, 'quantity': 10},
#    {'name': 'wine', 'price': 10.0, 'quantity': 5},
#]
# basic_backend.py
#items = list()  # global variable where we keep the data
#def create_items(app_items):
#    global items
#    items = app_items
#def create_item(name, price, quantity):
#    global items
#    items.append({'name': name, 'price': price, 'quantity': quantity})
# basic_backend.py
#def read_item(name):
#    global items
#    myitems = list(filter(lambda x: x['name'] == name, items))
#    return myitems[0]
##    global items
#    return [item for item in items]
# mvc_exceptions.py
#class ItemAlreadyStored(Exception):
#    pass
#class ItemNotStored(Exception):
#    pass
#import mvc_exceptions as mvc_exc
#items = list()
#def create_item(name, price, quantity):
#    global items
#    results = list(filter(lambda x: x['name'] == name, items))
#    if results:
#        raise mvc_exc.ItemAlreadyStored('"{}" already stored!'.format(name))
#    else:
#        items.append({'name': name, 'price': price, 'quantity': quantity})
#def create_items(app_items):
#    global items
#    items = app_items
#def read_item(name):
#    global items
#    myitems = list(filter(lambda x: x['name'] == name, items))
#    if myitems:
#        return myitems[0]
#    else:
#        raise mvc_exc.ItemNotStored(
#            'Can\'t read "{}" because it\'s not stored'.format(name))
#def read_items():
#    global items
#    return [item for item in items]
# basic_backend.py
#def update_item(name, price, quantity):
#    global items
    # Python 3.x removed tuple parameters unpacking (PEP 3113), so we have to do it manually (i_x is a tuple, idxs_items is a list of tuples)
#    idxs_items = list(
#        filter(lambda i_x: i_x[1]['name'] == name, enumerate(items)))
#    if idxs_items:
#        i, item_to_update = idxs_items[0][0], idxs_items[0][1]
#        items[i] = {'name': name, 'price': price, 'quantity': quantity}
#    else:
#        raise mvc_exc.ItemNotStored(
#            'Can\'t update "{}" because it\'s not stored'.format(name))
#def delete_item(name):
#    global items
    # Python 3.x removed tuple parameters unpacking (PEP 3113), so we have to do it manually (i_x is a tuple, idxs_items is a list of tuples)
#    idxs_items = list(
#        filter(lambda i_x: i_x[1]['name'] == name, enumerate(items)))
#    if idxs_items:
#        i, item_to_delete = idxs_items[0][0], idxs_items[0][1]
#        del items[i]
##raise mvc_exc.ItemNotStored(
  #          'Can\'t delete "{}" because it\'s not stored'.format(name))
# basic_backend.py
#def main():
#    my_items = [
#        {'name': 'bread', 'price': 0.5, 'quantity': 20},
#        {'name': 'milk', 'price': 1.0, 'quantity': 10},
#        {'name': 'wine', 'price': 10.0, 'quantity': 5},
#    ]

    # CREATE
#    create_items(my_items)
#    create_item('beer', price=3.0, quantity=15)
    # if we try to re-create an object we get an ItemAlreadyStored exception
    # create_item('beer', price=2.0, quantity=10)

    # READ
#    print('READ items')
#    print(read_items())
    # if we try to read an object not stored we get an ItemNotStored exception
    # print('READ chocolate')
    # print(read_item('chocolate'))
#    print('READ bread')
#    print(read_item('bread'))

    # UPDATE
#    print('UPDATE bread')
#    update_item('bread', price=2.0, quantity=30)
#    print(read_item('bread'))
    # if we try to update an object not stored we get an ItemNotStored exception
    # print('UPDATE chocolate')
    # update_item('chocolate', price=10.0, quantity=20)

    # DELETE
#    print('DELETE beer')
#    delete_item('beer')
    # if we try to delete an object not stored we get an ItemNotStored exception
    # print('DELETE chocolate')
    # delete_item('chocolate')
#    print('READ items')
#    print(read_items())

#if __name__ == '__main__':
#    main()
# model_view_controller.py
#import basic_backend
#import mvc_exceptions as mvc_exc
#class ModelBasic(object):
#    def __init__(self, application_items):
#        self._item_type = 'product'
#        self.create_items(application_items)
#    @property
#    def item_type(self):
#        return self._item_type
#    @item_type.setter
#    def item_type(self, new_item_type):
#        self._item_type = new_item_type
#    def create_item(self, name, price, quantity):
#        basic_backend.create_item(name, price, quantity)

#    def create_items(self, items):
#        basic_backend.create_items(items)

#    def read_item(self, name):
 #       return basic_backend.read_item(name)

#    def read_items(self):
#        return basic_backend.read_items()

#    def update_item(self, name, price, quantity):
#        basic_backend.update_item(name, price, quantity)

#    def delete_item(self, name):
#        basic_backend.delete_item(name)
# model_view_controller.py
#class View(object):
#    @staticmethod
#    def show_bullet_point_list(item_type, items):
#        print('--- {} LIST ---'.format(item_type.upper()))
#        for item in items:
#            print('* {}'.format(item))
#    @staticmethod
#    def show_number_point_list(item_type, items):
#        print('--- {} LIST ---'.format(item_type.upper()))
#        for i, item in enumerate(items):
#            print('{}. {}'.format(i+1, item))

#    @staticmethod
#    def show_item(item_type, item, item_info):
#        print('//////////////////////////////////////////////////////////////')
#        print('Good news, we have some {}!'.format(item.upper()))
#        print('{} INFO: {}'.format(item_type.upper(), item_info))
#        print('//////////////////////////////////////////////////////////////')

#    @staticmethod
#    def display_missing_item_error(item, err):
#        print('**************************************************************')
#        print('We are sorry, we have no {}!'.format(item.upper()))
#        print('{}'.format(err.args[0]))
#        print('**************************************************************')
#    @staticmethod
#    def display_item_already_stored_error(item, item_type, err):
#        print('**************************************************************')
#        print('Hey! We already have {} in our {} list!'
#              .format(item.upper(), item_type))
#        print('{}'.format(err.args[0]))
#        print('**************************************************************')
#    @staticmethod
#    def display_item_not_yet_stored_error(item, item_type, err):
#        print('**************************************************************')
#        print('We don\'t have any {} in our {} list. Please insert it first!'
#              .format(item.upper(), item_type))
#        print('{}'.format(err.args[0]))
#        print('**************************************************************')
#    @staticmethod
#    def display_item_stored(item, item_type):
#        print('++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++')
#        print('Hooray! We have just added some {} to our {} list!'
#              .format(item.upper(), item_type))
#        print('++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++')
 #   @staticmethod
#    def display_change_item_type(older, newer):
#        print('---   ---   ---   ---   ---   ---   ---   ---   ---   ---   --')
#        print('Change item type from "{}" to "{}"'.format(older, newer))
#        print('---   ---   ---   ---   ---   ---   ---   ---   ---   ---   --')
#    @staticmethod
#    def display_item_updated(item, o_price, o_quantity, n_price, n_quantity):
#        print('---   ---   ---   ---   ---   ---   ---   ---   ---   ---   --')
 #       print('Change {} price: {} --> {}'
 #             .format(item, o_price, n_price))
#        print('Change {} quantity: {} --> {}'
#              .format(item, o_quantity, n_quantity))
#        print('---   ---   ---   ---   ---   ---   ---   ---   ---   ---   --')
#    @staticmethod
#    def display_item_deletion(name):
#        print('--------------------------------------------------------------')
#        print('We have just removed {} from our list'.format(name))
#        print('--------------------------------------------------------------')
# model_view_controller.py
#class Controller(object):
#    def __init__(self, model, view):
#        self.model = model
#        self.view = view
#    def show_items(self, bullet_points=False):
#        items = self.model.read_items()
#        item_type = self.model.item_type
#        if bullet_points:
#            self.view.show_bullet_point_list(item_type, items)
#        else:
#            self.view.show_number_point_list(item_type, items)
#    def show_item(self, item_name):
#        try:
#            item = self.model.read_item(item_name)
#            item_type = self.model.item_type
#            self.view.show_item(item_type, item_name, item)
#        except mvc_exc.ItemNotStored as e:
#            self.view.display_missing_item_error(item_name, e)
#    def insert_item(self, name, price, quantity):
#        assert price > 0, 'price must be greater than 0'
#        assert quantity >= 0, 'quantity must be greater than or equal to 0'
#        item_type = self.model.item_type
#        try:
#            self.model.create_item(name, price, quantity)
#            self.view.display_item_stored(name, item_type)
#        except mvc_exc.ItemAlreadyStored as e:
#            self.view.display_item_already_stored_error(name, item_type, e)
#    def update_item(self, name, price, quantity):
#        assert price > 0, 'price must be greater than 0'
#        assert quantity >= 0, 'quantity must be greater than or equal to 0'
#        item_type = self.model.item_type
#        try:
#            older = self.model.read_item(name)
#            self.model.update_item(name, price, quantity)
#            self.view.display_item_updated(
#                name, older['price'], older['quantity'], price, quantity)
#        except mvc_exc.ItemNotStored as e:
#            self.view.display_item_not_yet_stored_error(name, item_type, e)
            # if the item is not yet stored and we performed an update, we have
            # 2 options: do nothing or call insert_item to add it.
            # self.insert_item(name, price, quantity)
#    def update_item_type(self, new_item_type):
#        old_item_type = self.model.item_type
#        self.model.item_type = new_item_type
#        self.view.display_change_item_type(old_item_type, new_item_type)
#    def delete_item(self, name):
#        item_type = self.model.item_type
#        try:
#            self.model.delete_item(name)
#            self.view.display_item_deletion(name)
#        except mvc_exc.ItemNotStored as e:
#            self.view.display_item_not_yet_stored_error(name, item_type, e)
# model_view_controller.py
#my_items = [
#    {'name': 'bread', 'price': 0.5, 'quantity': 20},
#    {'name': 'milk', 'price': 1.0, 'quantity': 10},
#    {'name': 'wine', 'price': 10.0, 'quantity': 5},
#]
#c = Controller(ModelBasic(my_items), View())
#--- PRODUCT LIST ---
#1. {'name': 'bread', 'price': 0.5, 'quantity': 20}
#2. {'name': 'milk', 'price': 1.0, 'quantity': 10}
#3. {'name': 'wine', 'price': 10.0, 'quantity': 5}
#--- PRODUCT LIST ---
#* {'name': 'bread', 'price': 0.5, 'quantity': 20}
#* {'name': 'milk', 'price': 1.0, 'quantity': 10}
#* {'name': 'wine', 'price': 10.0, 'quantity': 5}
#**************************************************************
#We are sorry, we have no CHOCOLATE!
#Can't read "chocolate" because it's not stored
#**************************************************************
#//////////////////////////////////////////////////////////////
#Good news, we have some BREAD!
#PRODUCT INFO: {'name': 'bread', 'price': 0.5, 'quantity': 20}
#//////////////////////////////////////////////////////////////
#**************************************************************
#Hey! We already have BREAD in our product list!
#"bread" already stored!
#**************************************************************
#++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
#Hooray! We have just added some CHOCOLATE to our product list!
#++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
#//////////////////////////////////////////////////////////////
#Good news, we have some CHOCOLATE!
#PRODUCT INFO: {'name': 'chocolate', 'price': 2.0, 'quantity': 10}
#//////////////////////////////////////////////////////////////
#---   ---   ---   ---   ---   ---   ---   ---   ---   ---   --
#Change milk price: 1.0 --> 1.2
#Change milk quantity: 10 --> 20
#---   ---   ---   ---   ---   ---   ---   ---   ---   ---   --
#**************************************************************
#We don't have any ICE CREAM in our product list. Please insert it first!
#Can't read "ice cream" because it's not stored
#**************************************************************
#**************************************************************
#We don't have any FISH in our product list. Please insert it first!
#Can't delete "fish" because it's not stored
#**************************************************************
#--------------------------------------------------------------
#We have just removed bread from our list
#--------------------------------------------------------------

#                                                 Домашняя  работа  4.08.24
#                        Задача№1
#class Singleton:
# _instance = None
#def __new__(cls):
# if not cls._instance:
#  cls._instance = super(Singleton, cls).__new__(cls)
#  return cls._instance
# Пример использования
#singleton_instance1 = Singleton()
#singleton_instance2 = Singleton()
#print(singleton_instance1 is singleton_instance2)
#                         Задача№2
#class Animal:
# def speak(self):
#  pass
#class Dog(Animal):
# def speak(self):
#  return "Woof!"
#class Cat(Animal):
# def speak(self):
#  return "Meow!"
#class AnimalFactory:
# def create_animal(self, animal_type):
#  if animal_type == "dog":
#  return Dog()
#elif animal_type == "cat":
#return Cat()
#else:
#return None
#factory = AnimalFactory()
#dog = factory.create_animal("dog")
#cat = factory.create_animal("cat")
#print(dog.speak()) # Вывод: Woof!
#print(cat.speak()) # Вывод: Meow!







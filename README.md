# Real_Calculator
print("*****Real Calculator*****")

print("-"*30)
list = ("Addition: +", "Subtraction: -", "Divide: /", "Multiplication: *", "Power: **", "Modules: %", "Quotient: //")

for i in list:
    print(i)

print("-"*30)
num1 = int(input("Enter the 1st Number: "))
operator = str(input("Enter the Operator: "))
num2 = int(input("Enter the 2nd Number: "))
print("-"*30)

def add(num1,num2):
    addition = num1 + num2
    print(f"{num1} {operator} {num2} = {addition} ")

def sub(num1,num2):
    subtraction = num1 - num2
    print(f"{num1} {operator} {num2} = {subtraction} ")

def mult(num1,num2):
    multiply = num1 * num2
    print(f"{num1} {operator} {num2} = {multiply} ")

def div(num1,num2):
    divide = num1 / num2
    print(f"{num1} {operator} {num2} = {divide} ")

def pwr(num1,num2):
    power = num1 ** num2
    print(f"{num1} {operator} {num2} = {power} ")

def mod(num1,num2):
    modulas = num1 % num2
    print(f"{num1} {operator} {num2} = {modulas} ")

def quot(num1,num2):
    quotient = num1 // num2
    print(f"{num1} {operator} {num2} = {quotient} ")

if operator == '+':
    print(add(num1,num2))

elif operator == '-':
    print(sub(num1,num2))

elif operator == '*':
    print(mult(num1,num2))

elif operator == '/':
    print(div(num1,num2))

elif operator == '**':
    print(pwr(num1,num2))

elif operator == '%':
    print(mod(num1,num2))

elif operator == '//':
    print(quot(num1,num2))

else:
    print("Invalid Type Error. ")

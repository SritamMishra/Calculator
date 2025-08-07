import math

def add(x, y):
    return x + y

def subtract(x, y):
    return x - y

def multiply(x, y):
    return x * y

def divide(x, y):
    if y == 0:
        return "Error: Division by zero"
    return x / y

def modulus(x, y):
    return x % y

def power(x, y):
    return x ** y

def square_root(x):
    return math.sqrt(x)

def logarithm(x):
    if x <= 0:
        return "Error: Logarithm undefined for 0 or negative"
    return math.log10(x)

def sine(x):
    return math.sin(math.radians(x))

def cosine(x):
    return math.cos(math.radians(x))

def tangent(x):
    return math.tan(math.radians(x))

def factorial(x):
    if x < 0:
        return "Error: Factorial undefined for negative numbers"
    return math.factorial(int(x))

def show_menu():
    print("\n===== Scientific Calculator =====")
    print("1. Addition")
    print("2. Subtraction")
    print("3. Multiplication")
    print("4. Division")
    print("5. Modulus")
    print("6. Power")
    print("7. Square Root")
    print("8. Logarithm (base 10)")
    print("9. Sine")
    print("10. Cosine")
    print("11. Tangent")
    print("12. Factorial")
    print("13. Exit")

a = float(input("Enter first number: "))
b = float(input("Enter second number: "))
show_menu()
choice = input("Choose operation (1-13): ")

if (choice == '13'):
        print("Thank you for using the calculator!")
        
    
if (choice == 1):
                print("Result:", add(a, b))
elif (choice == 2):
                print("Result:", subtract(a, b))
elif (choice == 3):
                print("Result:", multiply(a, b))
elif (choice == 4):
                print("Result:", divide(a, b))
elif (choice == 5):
                print("Result:", modulus(a, b))
elif (choice == 6):
                print("Result:", power(a, b))

        
            
elif (choice == 7):
                print("Result:", square_root(a,b))
elif (choice == 8):
                print("Result:", logarithm(a,b))
elif (choice == 9):
                print("Result:", sine(a,b))
elif (choice == 10):
                print("Result:", cosine(a,b))
elif (choice == 11):
                print("Result:", tangent(a,b))
elif (choice == 12):
                print("Result:", factorial(a,b))

else:
    print("Invalid choice. Please select between 1 and 13.")# programme

# Scientific-calculator-
Scientific Calculator is a Python program used to perform basic and advanced mathematical operations such as addition, subtraction, multiplication, division, power, square root, logarithm, and trigonometric calculations.
import math

print("===== SCIENTIFIC CALCULATOR =====")
print("1. Addition")
print("2. Subtraction")
print("3. Multiplication")
print("4. Division")
print("5. Power")
print("6. Square Root")
print("7. Logarithm")
print("8. Sin")
print("9. Cos")
print("10. Tan")

choice = int(input("Enter your choice: "))

if choice in [1, 2, 3, 4, 5]:
    a = float(input("Enter first number: "))
    b = float(input("Enter second number: "))

    if choice == 1:
        print("Result =", a + b)
    elif choice == 2:
        print("Result =", a - b)
    elif choice == 3:
        print("Result =", a * b)
    elif choice == 4:
        if b != 0:
            print("Result =", a / b)
        else:
            print("Cannot divide by zero")
    elif choice == 5:
        print("Result =", a ** b)

elif choice == 6:
    a = float(input("Enter a number: "))
    print("Result =", math.sqrt(a))

elif choice == 7:
    a = float(input("Enter a positive number: "))
    print("Result =", math.log(a))

elif choice in [8, 9, 10]:
    angle = float(input("Enter angle in degrees: "))
    radians = math.radians(angle)

    if choice == 8:
        print("Result =", math.sin(radians))
    elif choice == 9:
        print("Result =", math.cos(radians))
    elif choice == 10:
        print("Result =", math.tan(radians))

else:
    print("Invalid choice")

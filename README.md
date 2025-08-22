# Calculator

def add(x, y):
    return x + y 

def subtract(x, y):
    return x - y

def multiply(x, y):
    return x * y

def divide(x, y):
    return x / y

print("Select opreation.")
print("1.Add")
print("2.Subtract")
print("3.Multiply")
print("4.Divide")

while True:
    choice = input("Enter choice(1/2/3/4):")

    if choice in ('1', '2', '3', '4'):
        try:
            num1 = float(input("Enter the First Number: "))
            num2 = float(input("Enter the Second Number: "))
        except ValueError:

            print("Invalid input. Please enter a number.")
            continue

        if choice =='1':
            print(num1, "+", num2, "=", add(num1, num2))

        elif choice == '2':
            print(num1, "-", num2, "=", subtract(num1, num2))

        elif choice == '3':
            print(num1, "*", num2, "=", subtract(num1, num2))

        elif choice == '4':
            print(num1, "/", num2, "=", subtract(num1, num2))

        next_calculation =  input("Let's do next calculation ? (Yes/No): ")
        if next_calculation == "no":
            break
        else:
            print("invalid Input")
            

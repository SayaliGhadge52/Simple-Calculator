# Simple-Calculator
Using Python

def calculate():
    print("Choose operator (+,-,*,/):")
    mode = input()
    print("Choose first int:")
    x = int(input())
    print("Choose second int:")
    y = int(input())

    print("Your result:")
    if mode == "+":
        print(x + y)
    elif mode == "-":
        print(x - y)
    elif mode == "*":
        print(x * y)
    elif mode == "/":
        print(x / y)
    else:
        print("Invalid")
    again()

def again():
    cal_again = input("Do you want to calculate again? Y = yes or N = no: ")
   # Taking user input
    if cal_again.upper() == 'Y':
        calculate()
    elif cal_again.upper() == 'N':
        print('End')
    else:
        again()
calculate()

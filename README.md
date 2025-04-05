# PYTHONdef calculator():
    # Get user input
    num1 = float(input("Enter first number: "))
    num2 = float(input("Enter second number: "))
    operation = input("Enter operation (+, -, *, /): ")
    
    # Perform calculation based on operation
    if operation == '+':
        result = num1 + num2
        operation_name = "addition"
    elif operation == '-':
        result = num1 - num2
        operation_name = "subtraction"
    elif operation == '*':
        result = num1 * num2
        operation_name = "multiplication"
    elif operation == '/':
        if num2 == 0:
            print("Error: Division by zero is not allowed.")
            return
        result = num1 / num2
        operation_name = "division"
    else:
        print("Error: Invalid operation. Please use +, -, *, or /.")
        return
    
    # Display result
    print(f"{num1} {operation} {num2} = {result}")
    print(f"The {operation_name} of {num1} and {num2} is {result}.")

if __name__ == "__main__":
    print("Simple Calculator")
    print("=================")
    calculator()

# python-assignment-wk1
# Ask the user for two numbers and the desired operation
num1 = float(input("Enter the first number: "))
num2 = float(input("Enter the second number: "))
operation = input("Enter the operation (+, -, *, /): ")

# Perform the operation based on the user's input
if operation == "+":
    result = num1 + num2
elif operation == "-":
    result = num1 - num2
elif operation == "*":
    result = num1 * num2
elif operation == "/":
    # Check for division by zero
    if num2 != 0:
        result = num1 / num2
    else:
        result = "Error: Cannot divide by zero."
else:
    result = "Invalid operation."

# Display the result
print(f"The result of {num1} {operation} {num2} is: {result}")

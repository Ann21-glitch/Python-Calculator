# Function to perform the requested mathematical operation
def calculate(num1, num2, operation):
    if operation == '+':
        return num1 + num2
    elif operation == '-':
        return num1 - num2
    elif operation == '*':
        return num1 * num2
    elif operation == '/':
        if num2 != 0:  # Check to avoid division by zero
            return num1 / num2
        else:
            return "Error: Division by zero"
    else:
        return "Invalid operation"

# Main program
def main():
    # Get input from the user
    num1 = float(input("Enter the first number: "))
    num2 = float(input("Enter the second number: "))
    operation = input("Enter the operation (+, -, *, /): ")

    # Perform the calculation
    result = calculate(num1, num2, operation)

    # Display the result
    print(f"{num1} {operation} {num2} = {result}")

# Run the main program
if __name__ == "__main__":
    main()


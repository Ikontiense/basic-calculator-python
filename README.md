# 🧮 Basic Calculator in Python

This is a simple Python program that performs basic arithmetic operations:  
**Addition (+), Subtraction (-), Multiplication (*), and Division (/).**

---

## 🚀 Features
- Takes two numbers as input.
- Supports four operations: `+`, `-`, `*`, `/`.
- Handles division by zero errors.
- Validates user input.

# Basic Calculator Program with Loop

def calculator():
    print("🧮 Welcome to the Basic Calculator!")

    while True:
        try:
            num1 = float(input("\nEnter the first number: "))
            num2 = float(input("Enter the second number: "))
            operation = input("Enter an operation (+, -, *, /): ")

            if operation == "+":
                result = num1 + num2
            elif operation == "-":
                result = num1 - num2
            elif operation == "*":
                result = num1 * num2
            elif operation == "/":
                if num2 == 0:
                    print("❌ Error: Division by zero is not allowed.")
                    continue
                result = num1 / num2
            else:
                print("❌ Invalid operation! Please use +, -, *, or /.")
                continue

            print(f"✅ Result: {num1} {operation} {num2} = {result}")

        except ValueError:
            print("❌ Please enter valid numbers.")
            continue

        # Ask user if they want another calculation
        choice = input("\nDo you want to calculate again? (yes/no): ").lower()
        if choice != "yes":
            print("👋 Goodbye! Thanks for using the calculator.")
            break

calculator()

---
👉 Now, after each calculation, the program asks:
Do you want to calculate again? (yes/no)

## 💻 Example Usage
```bash
Enter the first number: 10  
Enter the second number: 5  
Enter an operation (+, -, *, /): +  

Output:  
10.0 + 5.0 = 15.0
Do you want to calculate again? (yes/no)

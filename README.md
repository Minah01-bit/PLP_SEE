def calculator():
    print("Basic Calculator")
    print("Operations available:")
    print("1. Addition (+)")
    print("2. Subtraction (-)")
    print("3. Multiplication (*)")
    print("4. Division (/)")
    print("5. Exit")

    while True:
        try:
            # Get user input
            choice = input("\nEnter operation number (1-5): ")
            
            if choice == '5':
                print("Exiting calculator. Goodbye!")
                break
            
            if choice not in ['1', '2', '3', '4']:
                print("Invalid choice. Please enter a number between 1 and 5.")
                continue
            
            num1 = float(input("Enter first number: "))
            num2 = float(input("Enter second number: "))
            
            # Perform calculation based on user choice
            if choice == '1':
                result = num1 + num2
                print(f"Result: {num1} + {num2} = {result}")
            elif choice == '2':
                result = num1 - num2
                print(f"Result: {num1} - {num2} = {result}")
            elif choice == '3':
                result = num1 * num2

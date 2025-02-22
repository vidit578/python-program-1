def is_armstrong_number(num):
    # Convert the number to a string to easily iterate over its digits
    num_str = str(num)
    # Calculate the number of digits
    num_digits = len(num_str)
    # Initialize a variable to store the sum of the digits raised to the power of num_digits
    armstrong_sum = 0
    
    # Iterate over each digit in the number
    for digit in num_str:
        # Convert the digit back to an integer and raise it to the power of num_digits
        armstrong_sum += int(digit) ** num_digits
        
    # Check if the sum equals the original number
    return armstrong_sum == num

# Example usage
number = int(input("Enter a number: "))
if is_armstrong_number(number):
    print(f"{number} is an Armstrong number.")
else:
    print(f"{number} is not an Armstrong number.")



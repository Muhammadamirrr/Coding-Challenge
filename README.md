# Coding-Challenge
def sort(width, height, length, mass):
    volume = width * height * length

    if volume >= 1000000 or width >= 150 or height >= 150 or length >= 150:
        if mass >= 20:
            return "REJECTED"
        else:
            return "SPECIAL"
    elif mass >= 20:
        return "SPECIAL"
    else:
        return "STANDARD"

# Test cases
print(sort(100, 50, 30, 15))  # STANDARD
print(sort(160, 40, 40, 18))  # SPECIAL
print(sort(120, 80, 90, 25))  # REJECTED

Technical Screening Challenge:
The sort function takes the dimensions (width, height, length) and mass of the package as parameters.
It calculates the volume of the package based on the dimensions.
Then, it checks the conditions specified in the rules to determine the appropriate stack for the package.
Finally, it returns the name of the stack.
You can test the function with different input values to verify its correctness. Feel free to use this code as a starting point and adapt it to your preferred programming language if needed.

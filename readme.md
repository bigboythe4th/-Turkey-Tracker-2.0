#my code
#turkey tracker calculator
#testing
def calculate_cooking_time(weight):
    if weight < 10:
        return weight * 20  # Assuming 20 minutes per pound for cooking time for smaller turkeys
    else:
        return weight * 15  # Assuming 15 minutes per pound for cooking time for larger turkeys
while True:
    try:
        turkey_weight = float(input("Enter the weight of the turkey in pounds: "))
        if turkey_weight <= 0:
            print("Please enter a valid weight for the turkey.")
            continue
        cooking_time = calculate_cooking_time(turkey_weight)
        print("The turkey will take", cooking_time, "minutes to cook.")
        break
    except ValueError:
        print("Invalid input. Please enter a number for the weight of the turkey.")
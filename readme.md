#my code
#turkey tracker calculator
#testing
#my code
#turkey tracker calculator
#testing
def calculate_cooking_time(weight):
    if weight < 10:
        return weight * 20  # 20 min for small 
    else:
        return weight * 15  # 15 min
while True:
    try:
        turkey_weight = float(input("Enter the weight of the turkey in pounds: "))
        if turkey_weight <= 0:
            print(" enter a real weight for the turkey.")
            continue
        cooking_time = calculate_cooking_time(turkey_weight)
        print("The turkey will take", cooking_time, "minutes to cook.")
        break
    except ValueError:
        print("Invalid input. Please enter a number for the weight of the turkey.")
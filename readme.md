#my code
#turkey tracker calculator
#testing
def calculate_cooking_time(weight):
    if weight < 10:
        return weight * 20  # Assuming 20 minutes per pound for cooking time for smaller turkeys
    else:
        return weight * 15  # Assuming 15 minutes per pound for cooking time for larger turkeys


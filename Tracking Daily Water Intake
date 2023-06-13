# Example 1: Tracking Daily Water Intake
# Function to get user input and validate the input format
def get_user_input(prompt):
    while True:
        try:
            value = float(input(prompt))
            if value >= 0:
                return value
            else:
                print("Please enter a non-negative value.")
        except ValueError:
            print("Please enter a valid number.")

# Function to display output
def display_output(label, value):
    print(label, value)

# Initialize variables
total_water_intake = 0
recommended_daily_intake = 2000
alert_percentage = 70  # Set the percentage at which you want to trigger the alert

# Prompt the user to enter the amount of water consumed in the morning
morning_water = get_user_input("Enter the amount of water consumed in the morning: ")

# Add the morning water intake to the total
total_water_intake += morning_water

# Prompt the user to enter the amount of water consumed in the afternoon
afternoon_water = get_user_input("Enter the amount of water consumed in the afternoon: ")

# Add the afternoon water intake to the total
total_water_intake += afternoon_water

# Prompt the user to enter the amount of water consumed in the evening
evening_water = get_user_input("Enter the amount of water consumed in the evening: ")

# Add the evening water intake to the total
total_water_intake += evening_water

# Calculate the percentage of recommended daily intake achieved
percentage_achieved = (total_water_intake / recommended_daily_intake) * 100

# Display the total water intake and percentage achieved
display_output("Total water intake:", total_water_intake)
display_output("Percentage achieved:", percentage_achieved)

# Check if the percentage achieved reaches the alert threshold
while percentage_achieved < alert_percentage:
    additional_water = get_user_input("Enter additional amount of water consumed: ")
    total_water_intake += additional_water
    percentage_achieved = (total_water_intake / recommended_daily_intake) * 100

    # Display the updated total water intake and percentage achieved
    display_output("Total water intake:", total_water_intake)
    display_output("Percentage achieved:", percentage_achieved)

    # Check if the percentage achieved reaches the alert threshold
    if percentage_achieved >= alert_percentage:
        print("Alert: You have reached", alert_percentage, "% of your recommended daily water intake!")
        break
# End of program

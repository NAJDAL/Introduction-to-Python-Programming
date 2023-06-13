# Example 2: Hydration Reminder and Recommendation
# Function to calculate the recommended daily water intake
def calculate_daily_intake(age, weight, activity_level):
    # Add your logic to calculate the recommended daily water intake based on the provided parameters
    # Placeholder implementation
    return 2000

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

# Function to check if the user wants to end the program
def user_wants_to_end():
    response = input("Do you want to end the program? (yes/no): ")
    return response.lower() == "yes"

# Prompt the user to enter their age, weight, and activity level
age = get_user_input("Enter your age: ")
weight = get_user_input("Enter your weight: ")
activity_level = get_user_input("Enter your activity level: ")

# Calculate the recommended daily water intake based on user input
recommended_daily_intake = calculate_daily_intake(age, weight, activity_level)

# Initialize variables
total_water_intake = 0  # Total amount of water consumed since the last reminder
current_percentage_achieved = 0  # Current percentage of recommended daily intake achieved
reminder_interval = 2  # Interval between reminders in hours

# Display the recommended daily water intake
display_output("Recommended daily intake:", recommended_daily_intake)

# Enter a loop for hydration reminders
while True:
    # Display reminder to drink water
    display_output("Reminder: Drink water", "")

    # Prompt the user to enter the amount of water consumed since the last reminder
    consumed_water = get_user_input("Enter the amount of water consumed since the last reminder: ")

    # Add the consumed water to the total
    total_water_intake += consumed_water

    # Calculate the current percentage achieved
    current_percentage_achieved = (total_water_intake / recommended_daily_intake) * 100

    # Display the total water intake and current percentage achieved
    display_output("Total water intake:", total_water_intake)
    display_output("Current percentage achieved:", current_percentage_achieved)

    # Check if the user wants to end the program
    if user_wants_to_end():
        break

# End of program

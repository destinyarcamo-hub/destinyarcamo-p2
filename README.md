def calculate_average(score1, score2, score3):
    average = (score1 + score2 + score3) / 3
    return average

number_of_students = int(input("How many students? "))

while number_of_students < 3:
 print("Please enter at least 3 students.")
 number_of_students = int(input("How many students? "))

for student in range(number_of_students):

print("\nStudent", student + 1)
name = input("Enter name: ")

activity1 = float(input("Activity 1: "))
activity2 = float(input("Activity 2: "))
activity3 = float(input("Activity 3: "))

average = calculate_average(activity1, activity2, activity3)

if average >= 90:
status = "Excellent"
elif average >= 80:
status = "Very Good"
elif average >= 75:
status = "Passed"
else:
status = "Failed"

print("Name:", name)
print("Activity 1:", activity1)
print("Activity 2:", activity2)
print("Activity 3:", activity3)
print("Average:", round(average, 2))
print("Status:", status)

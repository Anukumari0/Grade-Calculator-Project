#Student Grade Calculator

print("===== STUDENT GRADE CALCULATOR =====")

# Taking input from the user
assignment = float(input("Enter Assignment Marks (out of 100): "))
lab = float(input("Enter Lab Marks (out of 100): "))
mid = float(input("Enter Midterm Marks (out of 100): "))
final = float(input("Enter Final Exam Marks (out of 100): "))
attendance = float(input("Enter Attendance Marks (out of 10): "))

# Calculating total marks
total = assignment * 0.25 + lab * 0.25 + mid * 0.20 + final * 0.25 + attendance

# Calculating percentage
percentage = (total / 110) * 100   # Total max marks = 110

# Grade calculation using if-elif-else
if percentage >= 90:
    grade = "A"
elif percentage >= 80:
    grade = "B"
elif percentage >= 70:
    grade = "C"
elif percentage >= 60:
    grade = "D"
else:
    grade = "F"

# Final Output
print("\n=========== RESULT ===========")
print(f"Assignment Marks : {assignment}")
print(f"Lab Marks        : {lab}")
print(f"Midterm Marks    : {mid}")
print(f"Final Marks      : {final}")
print(f"Attendance       : {attendance}/10")
print("-------------------------------")
print(f"Total Marks      : {total:.2f} / 110")
print(f"Percentage       : {percentage:.2f}%")
print(f"Final Grade      : {grade}")
print("================================")



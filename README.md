# CODETECH-task2
Name-Sneha Mote
Company-CODETECH IT SOLUTION
ID-CT08FRK
Domain-Python Programming
Duration dec to jan 2025
1. Purpose of the Program

The program is designed to:

Add/Update Grades: Allows the user to input grades for various subjects.

Display Grades: Shows all recorded grades, calculates the average, and displays the corresponding letter grade.

Exit: Allows the user to exit the program.



---

2. Structure of the Program

a. add_grade(grades)

This function:

Takes a dictionary grades as input to store grades for each subject.

Prompts the user to enter a subject name and a grade (as a number between 0 and 100).

Validates the input to ensure the grade is numeric and within the allowed range.

Adds or updates the grade for the given subject in the dictionary.


Example:

grades = {}
add_grade(grades)  # User enters "Math" and 85
# grades = {"Math": 85}


---

b. calculate_average(grades)

This function:

Calculates the average of all grades stored in the grades dictionary.

If no grades are available, it prints a message and returns 0.


Example:

grades = {"Math": 85, "Science": 90}
average = calculate_average(grades)  # average = (85 + 90) / 2 = 87.5


---

c. display_grades(grades)

This function:

Displays each subject and its grade from the grades dictionary.

Calls calculate_average(grades) to compute the average grade.

Converts the average to a letter grade using get_letter_grade().


Example:

grades = {"Math": 85, "Science": 90}
display_grades(grades)
# Output:
# Math: 85.00
# Science: 90.00
# Average Grade: 87.50
# Letter Grade: B


---

d. get_letter_grade(average)

This function:

Converts the numeric average grade to a letter grade:

A: 90–100

B: 80–89

C: 70–79

D: 60–69

F: Below 60



Example:

average = 87.5
letter_grade = get_letter_grade(average)  # letter_grade = "B"


---

e. main()

This function:

Runs the program and provides a menu for user interaction:

1. Add/Update a Grade.


2. Display Grades.


3. Exit.



Calls the appropriate function based on the user’s choice.

Continuously displays the menu until the user chooses to exit.


Example:

# Example run of main():
# User selects option 1: Adds grade
# User selects option 2: Displays grades
# User selects option 3: Exits the program


---

3. How the Program Works

1. Initialization:

The grades dictionary is initialized as empty to store subject-grade pairs.



2. Input and Validation:

The add_grade() function ensures that the input grade is numeric and between 0 and

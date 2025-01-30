# student management system
#student list(name,age,roll number)

students = []
unique_rolls = set()

#function to add student

def add_student(Name, Age, Roll):
    if Roll in unique_rolls:
        print("Roll number already exists! Please enter a unique roll number.")
    else:
        students.append((Name,Age,Roll)) #Tuple to added lists
        unique_rolls.add(Roll) # Roll number added to set
        print("Student added successfully")

        #Function to display all student
def display_students():
    if not students:
        print("No students found")
    else:
        print("\n Student list:")
        for i, student in enumerate(students, start=1):
            print(f"{1}. Name: {student[0]}, Age: {student[1]}, Roll Number: {student[2]}")

#Function to search for a student by roll number

def search_student(Roll):
    for student in students:
        print(" \n student found:")
        print(f"Name: {student[0]}, Age: {student[1]}, Roll number: {student[2]}")
        return
    print("Student not found.")
    return
#Main program Loop
while True:
     print("\n 1. Add student")
     print(" 2. Display students")
     print(" 3. Search student by roll number")
     print("4 . exit")

     choice = input("Enter your choice:")
     if choice == "1":
         Name = input("Enter student name:")
         Age = int(input("Enter student age:"))
         Roll = int(input("Enter student roll number:"))
         add_student(Name,Age,Roll)
     elif choice == "2":
         display_students()
     elif choice == "3":
         Roll = int(input("Enter student roll number to search:"))
         search_student(Roll)
     elif choice == "4":
         print("Exiting program")
         break
     else:
         print("Invalid choice. Please enter a valid choice.")


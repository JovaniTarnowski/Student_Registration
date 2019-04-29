student_list = []


def create_student():

        student_name = input("Please enter your name: ")
        student_data = {
            'name': student_name,
            'marks': []
        }
        return student_data


def append_student(student, mark):
    student['marks'].append(mark)


def calculate_average_mark(student):
    number = len(student['marks'])
    if number == 0:
        return 0
    total = sum(student['marks'])
    return total / number


def print_student_details(student):
    print("Students Name: {} Marks: {} Average: {} ".format(student['name'], student['marks'],
                                                            calculate_average_mark(student)))


def all_students_details(student_list):
    for i, student in enumerate(student_list):
        print("ID: {}". format(i))
        print_student_details(student)


def menu():
    selection = input("enter 'p' to print,"
                      "'s' to add, "
                      "'a' to add a mark"
                      "'or' to quit")
    while selection != 'q':
        if selection == 'p':
            print_student_details(student_list)
        elif selection == 's':
            student_list.append(create_student())
        elif selection == 'a':
            student_id = int(input("Enter Student ID: "))
            student = student_list[student_id]
            new_mark = int(input(" enter the new mark"))
            append_student(student, new_mark)

        selection = input("enter 'p' to print,"
                          "'s' to add, "
                          "'a' to add a mark"
                          "'or' to quit")
menu()



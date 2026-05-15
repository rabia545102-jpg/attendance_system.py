def attendance_report(students, attendance):

    total = len(students)
    present = 0
    absent = 0

    for student in students:
        if attendance[student] == "Present":
            present += 1
        else:
            absent += 1

    percentage = (present / total) * 100

    print("Total Students:", total)
    print("Present:", present)
    print("Absent:", absent)
    print("Attendance Percentage:", percentage, "%")


students = ["Ayesha", "Rahul", "Zoya", "Ali"]

attendance = {
    "Ayesha": "Present",
    "Rahul": "Absent",
    "Zoya": "Present",
    "Ali": "Present"
}

attendance_report(students, attendance)

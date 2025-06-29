 student_marks = {}

n = int(input("Enter number of students: "))
for _ in range(n):
    name = input("Enter student name: ")
    marks = int(input("Enter marks: "))
    student_marks[name] = marks

print("\nStudent Marks:")
for name, marks in student_marks.items():
    print(name, ":", marks)


list[start:stop:step]
print(numbers[1:4])     # [20, 30, 40]
print(numbers[:3])      # [10, 20, 30]
print(numbers[3:])      # [40, 50, 60, 70]
print(numbers[::2])     # [10, 30, 50, 70]
print(numbers[::-1])    # [70, 60, 50, 40, 30, 20, 10] (reversed list)
print(numbers[-4:-1])   # [40, 50, 60]



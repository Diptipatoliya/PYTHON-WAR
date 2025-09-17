# To-Do List Project in Python

tasks = []

def show_menu():
    print("\n--- To-Do List Menu ---")
    print("1. View Tasks")
    print("2. Add Task")
    print("3. Remove Task")
    print("4. Exit")

def view_tasks():
    if len(tasks) == 0:
        print("No tasks found! ✅")
    else:
        print("\nYour Tasks:")
        for i, task in enumerate(tasks, start=1):
            print(f"{i}. {task}")

def add_task():
    task = input("Enter a new task: ")
    tasks.append(task)
    print(f"Task '{task}' added successfully! 📝")

def remove_task():
    view_tasks()
    try:
        task_no = int(input("Enter task number to remove: "))
        removed = tasks.pop(task_no - 1)
        print(f"Task '{removed}' removed successfully! ❌")
    except (ValueError, IndexError):
        print("Invalid task number!")

while True:
    show_menu()
    choice = input("Enter your choice (1-4): ")

    if choice == '1':
        view_tasks()
    elif choice == '2':
        add_task()
    elif choice == '3':
        remove_task()
    elif choice == '4':
        print("Goodbye! 👋")
        break
    else:
        print("Invalid choice! Please try again.")

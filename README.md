## 📌 Run this command from your project's root directory
- For Mac :
```bash
java -cp "out:lib/*" attendance.ui.MainFrame
```

- Window:
```bash
java -cp "out;lib/*" attendance.ui.MainFrame
```
## 🌟 What is an Attendance Management System?
An Attendance Management System is a digital tool used to track the presence of individuals, such as students or staff. It automates record-keeping to replace manual paper methods, ensuring accuracy and saving time.

## 🌟 Scope of this System
This application allows an administrator to perform essential user management tasks:
- Add, Edit, and Delete User profiles, Class, Attendance.
- View all records in a single list and details record.
- Search for specific users by name.

## 🌟 Objectives of the System
This system is designed to overcome the challenges of manual record-keeping by achieving the following key objectives:
- Automate Data Handling
To replace slow and error-prone manual entry with an automated process. The system streamlines the tasks of adding, updating, and deleting records, minimizing manual labor and improving overall data management.
- Provide Easy GUI-Based Interaction
To offer a clean, intuitive, and user-friendly Graphical User Interface (GUI). This ensures that the administrator can interact with the system effortlessly, managing all records without needing complex commands or extensive training.
- Improve Search and Filtering of Data
To deliver a fast and effective search function. This allows the administrator to instantly locate any student, teacher, or staff record by name, drastically cutting down the time spent sifting through paper files or spreadsheets.
- Maintain Secure and Structured Records
To establish a centralized and structured database for all personnel information. This guarantees data consistency, enhances security, and provides a reliable foundation for managing and protecting valuable records, unlike scattered and vulnerable manual files.

## 🌟 Testing & Quality Assurance
1. Testing Approach
Our testing strategy involved multiple layers to ensure the application was robust and reliable.
- Unit Testing
Focused on the backend DatabaseHelper class. Each method (e.g., addEmployee, getAllEmployees) was individually tested to verify it performed the correct SQL operations and handled data correctly.
- GUI Testing
Manually tested all user interface elements. This included clicking buttons, entering data into forms, and selecting table rows to confirm that all events were handled properly and that the UI updated as expected after each action.
- Sample Test Case
Case: Add a new employee with valid data.
Action: Filled in all text fields and clicked the "Add Employee" button.
Expected Result: The new employee appears in the table, and the input fields are cleared.
Status: Passed.

2. Major Bug Found & Resolved
- Bug Identified:
The "Update" and "Delete" buttons would remain enabled even after an operation was completed. Clicking them again without selecting a new user could cause an application error.
- Resolution:
The code was improved to automatically disable these buttons after each successful update or deletion. The buttons are now only re-enabled when a user explicitly selects a new row from the table, preventing accidental errors.

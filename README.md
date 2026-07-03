# Student's Scores and Reporting System

**Course:** CTIP 152 at Stadio (Private University)
**Department:** School of Information Technology  

---

## 📌 Project Overview
A Python command-line application that allows for **Student's Scores and Reporting System**. Student profiles dataset can be managed, allowing educators or administrators to track student's marks, averages, pass and fail status', calculate grades, edit student lists and create statistical class reports. 

Data integrity is ensured by the program. The data undergoes strict data validation and prevents crashes.

## 🚀 Features
1. **Search Student Records:** Instantly look up a student's profile, full name, and test scores using their unique Student ID.
2. **Add New Students:** Dynamically insert new students into the system with built-in format checks for IDs, full names, and score boundaries.
3. **Delete Student Records:** Safely remove a student's profile from the dataset using their ID.
4. **Identify Performance Tiers:** Categorize students into Performance Tiers (Distinction, Pass, Fail).
5. **Class Statistics & Analytics:** Calculate total class averages, track overall pass rates, and find the highest and lowest performing students.
6. **Comprehensive Class Report:** Display a cleanly formatted tabular overview of the entire classroom's progress.

---

## 📁 Dataset Structure
The program initializes and manages an in-memory dictionary. Each student profile is structured as follows:

```python
students = {
    "ST001": {
        "name": "Alice Smith",
        "scores": [88, 91, 84]
    },
    # Additional student records...
}
```

---

## 🛠️ System Functions
The script is organized into the following core functions:

*   `addStudent()`: Validates and appends a new student ID, full name, and initial score to the database.
*   `verifyStudentID(studentInfo)`: Core validation engine ensuring IDs match proper formatting criteria (minimum length, containing uppercase letters and digits).
*   `search_student()`: Finds and prints matching student details with built-in retry logic.
*   `calculate_average()`: Loops through the active dataset to compute individual averages, group student performance tiers, and display data in a tabular summary.

---

## 💻 How To Run the Project

### Prerequisites
*   Make sure you have Python 3.x installed on your computer.

### Step-by-Step Execution
1. Download or copy the python script file (e.g., `student_system.py`).
2. Open your terminal, command prompt, or preferred IDE.
3. Navigate to the folder containing your script.
4. Run the file using the terminal command:
   ```bash
   python student_system.py
   ```

---

## ⚠️ Input Validation Rules
To keep data reliable, the program enforces these mandatory rules during data entry:
*   **Student ID:** Must contain uppercase letters, digits, and span a minimum of 5 total characters (e.g., `ST079`).
*   **Student Name:** Must be at least 2 characters long and include a space separating the first and last name.

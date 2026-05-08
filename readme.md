# Student Management System 🎓

A desktop application built with Python and PyQt6 for managing student records simply and efficiently.

---

## Features

- Add new student records with name, course and mobile number
- Edit existing student records
- Delete student records
- Search for students by name
- Data stored locally using SQLite
- Clean interface with toolbar, menu bar and dynamic status bar

---

## Requirements

- Python 3.x
- PyQt6
- SQLite3 (included with Python)

---

## Installation

1. **Clone or download the repository:**
   ```
   git clone https://github.com/yourusername/student-management-system.git
   ```

2. **Navigate to the project directory:**
   ```
   cd student-management-system
   ```

3. **Install dependencies:**
   ```
   pip install PyQt6
   ```

4. **Run the application:**
   ```
   python main.py
   ```

---

## Database Setup

The application automatically creates a local `database.db` SQLite file on first run. Ensure your database contains a `students` table with the following structure:

```sql
CREATE TABLE students (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    name TEXT,
    course TEXT,
    mobile TEXT
);
```

---

## How To Use

| Action | How |
|---|---|
| Add a student | File → Add Student or toolbar icon |
| Search for a student | Edit → Search or toolbar icon |
| Edit a student | Click a row → Edit Record button in status bar |
| Delete a student | Click a row → Delete Record button in status bar |

---

## Project Structure

```
student-management-system/
│
├── main.py               # Main application file
├── database.db           # SQLite database (auto-created)
├── icons/
│   ├── add.png           # Add student toolbar icon
│   └── search.png        # Search toolbar icon
└── README.md             # This file
```

---

## Built With

- [Python 3](https://www.python.org/) - Programming language
- [PyQt6](https://pypi.org/project/PyQt6/) - GUI framework
- [SQLite3](https://www.sqlite.org/) - Local database

---

## Author

Built by [Your Name]

---

## License

This project is open source and available under the [MIT License](LICENSE).
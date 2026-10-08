# mysql-database
Doctor summary (to see all details):
[✓] Flutter
[✓] Windows Version
[✓] Android toolchain
[✓] Chrome
[✓] Visual Studio
[✓] Connected device
[✓] Network resources
Creating project my_first_app...
Running pub get...
...
All done!
mysql -u root -p
CREATE DATABASE school;
CREATE TABLE students (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    email VARCHAR(150) UNIQUE,
    enrolled_on DATE
);
INSERT INTO students (name, email, enrolled_on)
VALUES
('John Doe', 'john@example.com', '2026-10-01'),
('Jane Smith', 'jane@example.com', '2026-10-02');
SELECT * FROM students;
+----+------------+------------------+-------------+
| id | name       | email            | enrolled_on |
+----+------------+------------------+-------------+
|  1 | John Doe   | john@example.com | 2026-10-01  |
|  2 | Jane Smith | jane@example.com | 2026-10-02  |
+----+------------+------------------+-------------+
CREATE DATABASE school;

USE school;

CREATE TABLE students (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    email VARCHAR(150) UNIQUE,
    enrolled_on DATE
);

INSERT INTO students (name, email, enrolled_on)
VALUES
('John Doe', 'john@example.com', '2026-10-01'),
('Jane Smith', 'jane@example.com', '2026-10-02');

SECREATE USER 'school_app'@'localhost'
IDENTIFIED BY 'StrongPassword123!';

GRANT SELECT, INSERT, UPDATE, DELETE
ON school.*
TO 'school_app'@'localhost';

FLUSH PRIVILEGES;LECT * FROM students;
.\venv\Scripts\Activate.ps1
mkdir python_setup_lab
cd python_setup_lab
python -m venv venv
venv\Scripts\activate
pip install requests
pip list
pip freeze > requirements.txt
Section 1: Task 1 - Flutter & Dart Setup

Section 2: Task 2 - MySQL Database Management

Section 3: Task 3 - Python Virtual Environment

Section 4: Task 4 - VS Code Workspace Screenshot
CREATE DATABASE school;
USE school;
SELECT * FROM students;




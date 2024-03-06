-- Create table for students
CREATE TABLE Students (
    student_id INT PRIMARY KEY,
    first_name VARCHAR(50),
    last_name VARCHAR(50),
    date_of_birth DATE,
    email VARCHAR(100),
    phone_number VARCHAR(15)
);

-- Create table for courses
CREATE TABLE Courses (
    course_id INT PRIMARY KEY,
    course_name VARCHAR(100),
    instructor VARCHAR(100)
);

-- Create table for student enrollment in courses
CREATE TABLE StudentCourses (
    student_id INT,
    course_id INT,
    FOREIGN KEY (student_id) REFERENCES Students(student_id),
    FOREIGN KEY (course_id) REFERENCES Courses(course_id),
    PRIMARY KEY (student_id, course_id)
);

-- Create table for student grades
CREATE TABLE Grades (
    student_id INT,
    course_id INT,
    grade DECIMAL(5, 2),
    FOREIGN KEY (student_id) REFERENCES Students(student_id),
    FOREIGN KEY (course_id) REFERENCES Courses(course_id),
    PRIMARY KEY (student_id, course_id)
);

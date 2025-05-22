### Finals-Lab-Task-3.1
# Using MYSQL CLAUSEREADME
## Instructions:
1. Create a database named online_courseDB
2. Use the online_courseDB
3. Copy and paste the initial query then perform the SELECT statements required for each
problems in the figure below: (download onlineCourse.sql file)

create database courses;
use courses;

CREATE TABLE courses (
    id INT AUTO_INCREMENT PRIMARY KEY,
    course_name VARCHAR(255) NOT NULL,
    category VARCHAR(100) NOT NULL,
    enrollment_limit INT NOT NULL,
    students_enrolled INT NOT NULL
);

INSERT INTO courses (course_name, category, enrollment_limit, students_enrolled)
VALUES
   
    ('Data Science', 'Technology', 50, 45),
    
    ('Graphic Design', 'Arts', 30, 25),
    
    ('Digital Marketing', 'Business', 40, 35),
   
    ('Introduction to Python', 'Technology', 100, 90),
    
    ('Creative Writing', 'Literature', 25, 20),
   
    ('UX/UI Design', 'Arts', 50, 40),
   
    ('Project Management', 'Business', 60, 55),
    
    ('Artificial Intelligence', 'Technology', 50, 48),
    
    ('Public Speaking', 'Communication', 30, 28),
    
    ('Photography', 'Arts', 25, 18),
    
    ('Web Development', 'Technology', 75, 70),
    
    ('SEO Strategies', 'Business', 30, 29),
    
    ('Blockchain Basics', 'Technology', 50, 50),
    
    ('Accounting 101', 'Business', 45, 40),
    
    ('Film Editing', 'Arts', 35, 33),
    
    ('Machine Learning', 'Technology', 60, 55),
    
    ('Speech Writing', 'Communication', 20, 15),
    
    ('Interior Design', 'Arts', 40, 38),
    
    ('Leadership Training', 'Business', 50, 48),
    
    ('Cybersecurity', 'Technology', 70, 65);
    
    SELECT * FROM courses
    WHERE students_enrolled < enrollment_limit;
    
    SELECT category, SUM(students_enrolled) AS total_enrolled
    FROM courses
    GROUP BY category;
    
    SELECT * FROM courses
   WHERE students_enrolled = enrollment_limit;
    
    SELECT SUM(students_enrolled) AS total_students_enrolled
    FROM courses;
    
    SELECT * FROM courses
    ORDER BY students_enrolled asc;
    
# Sample output
![Image](https://github.com/user-attachments/assets/d31db1aa-97c2-4032-8d29-69012ca2999b)
![Image](https://github.com/user-attachments/assets/e8c54a62-5b07-4152-96e3-8d913f033031)
## Sample output
![Image](https://github.com/user-attachments/assets/a31f6d2c-773a-43ea-8aa6-f7bd848729f4)
![Image](https://github.com/user-attachments/assets/e6ae8fb5-5f4b-433b-9e59-487d2c0c1e11)
## Sample output
![Image](https://github.com/user-attachments/assets/46a3a3dc-424a-4a95-b219-3452d56b7451)
![Image](https://github.com/user-attachments/assets/90278198-061e-42db-a57d-bc4369547236)
## Sample output
![Image](https://github.com/user-attachments/assets/833a650d-47d9-4727-aa0e-4c0ac1d9d5cb)
![Image](https://github.com/user-attachments/assets/a0b650df-00ae-4044-82ff-60ebf0ef7042)
## Sample output
![Image](https://github.com/user-attachments/assets/f703e8a6-0a03-477b-bdcf-9856006f615d)
![Image](https://github.com/user-attachments/assets/21d3d3dc-f738-4701-8cdd-c45533499a22)

 <a href="https://chan-edm.github.io/README/" class="btn">BACK TO PORTFOLIO</a>
    <a href="https://chan-edm.github.io/Finals-Lab-Task-5/" class="btn">CONTINUE TO LEARN</a>

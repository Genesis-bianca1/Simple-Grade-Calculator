To understand the login, open files in the following order:

    connect_database.php
    login.php
    logout.php
    index.php
    login_val.js
    module_credits.php
    enter_marks.php
    validation.js
    process_marks.php
    marks_results.php



The 'grading_system' database schema in 3NF:

Table ‘Student’:
student_id (PK), forename, surname,  passcode, repeated_passcode, course_code (FK).

Table ‘Module’:
course_code (FK), module_code (PK), module_name, credits.

Table ‘Marks’:
student_id (PK), module_code (FK), mark, grade.

Table ‘GPA’:
student_id (FK), average_mark.

Table ‘Course’:
course_code(PK), course_name.

Table ‘Classification’:
student_id (FK), award (FK), classification.

Table ‘Award’:
award (PK), total_credits, course_code(FK).


Functions of the system:
1. Secure and encrypted Login
2. Redirection to the 'Enter Marks' table page
3. Enter the appropriate marks of students' registered modules
4. 'Calculate Results' button performs the next 2 functions
5. Mark is translated into grades
6. Award based on degree criteria is revealed
7. Results above are displayed on a new page as a 'Results' table.
8. Log  out and delete session's data

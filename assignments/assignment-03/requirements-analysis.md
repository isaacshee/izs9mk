Assignment 3 - Requirements Analysis
Name: Isaac Shee
Pawprint: izs9mk

Step 1: Identify the different types of Users of the software system
The software will handle at least 3 different types of users namely:
  1. Instructor
  2. TA
  3. Student

Step 2: Activities each user type will perform with the software (User Requirements)
For Instructor: 1. Ability to upload lecture notes, assignments, quizzes etc. using the software for students.
                2. Ability to grade or review said assignments, quizzes or tests of every student taking the course.
                3. Ability to set due dates on any assignment or activiy.
                4. Ability to update or delete anything that has been uploaded.
                5. Ability to send announcements to all students participating in the course.
                6. Ability to create and manage sections for labs or groups.
                
For TA:         1. Ability to review and grade assignments uploaded by students
                2. Ability to upload and update assignments.
                3. Ability to send announcements to all students participating in the course.
                4. Ability to host discussions or labs 
        
For Students:   1. Ability to access course materials that have been uploaded (i.e. lecture notes, lab notes).
                2. Ability to access and submit assignments.
                3. Ability to review grades that have been issued.
                4. Ability to post on discussion boards.
                
Step 3: Identifying relevant data and constraints within the system
For all Instructor Activities: 
Entities: Assignment(assignmentID, type, title, date_uploaded, due_date), Grade(studentID, assignmentID, grade, date),
          Announcement(title, message, date), Lab_section(labID, time, location), Group(groupID, members), 
          Discussion(date, time, message)
          
Constraints: 1. A student cannot be assigned to more than one group
             2. A student cannot belong to more than one lab section
             
For all TA Activities:
Entities: Assignment(assignmentID, type, title, date_uploaded, due_date), Grade(studentID, assignmentID, grade, date),
          Announcement(title, message, date), Lab_section(labID, time, location), Discussion(date, time, message)

Constraints: 1. TA should not be able to upload any assignment without Instructor's approval
             2. If multiple TAs, they should only be able to grade students in lab sections assigned to them

For all Student Activities:
Entities: Assignment(date, time, submission), Grade(assignmentID, grade, avg), Discussion(date, time, message)

Constraints: 1. Once a due date has past, a student cannot submit the assignment or will have an automatic penalty to the grade of the                   assignment
             2. The student must only be able to post to their respective groups or to the class discussion
              
Step 4: Identifying System constraints and requirements
  -The system should operate based on the existing student portal software by being intergrated into it.
  -The system would require adequate storage of atleast ~500 MB on a local platform.
  -The system would require internet connection.

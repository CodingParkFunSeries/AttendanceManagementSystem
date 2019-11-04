# Attendance Managemnet System 

## Scope 
Track attendance of the students of schools.

## Extended scope
- System should be able to track attendance for universities, where attendance is being tracked per subject instead of per day.
- System should also work fine where manager want to track attendance for their employees. It could be used to trace the attendance of
the teachers too. 
- Students will be awarded badges for regularity of his attendance. 

## Roles
- Students
- Class Teacher/Owner ( We don't care about other teachers for MVP) 
- Admin

## Admin Role
- Admin will register in our application and create a school.
- Admin can create classrooms
- Class can be activated and deactived. Ideally a student should belong to only one active class at a time. Considering it as session.
- Admin should be able to create class, students and assign student to a class. 
- Admin can assgin teacher and student to class. A student can be assigned to only one active class at at time. 
- Admin can create leaves list in the system, also he can mention that working days for the schools. Total attendance will 
be considered for working days only.

## Teachers
- Teachers should be able mark attendance of the students who belongs to same class in which teacher is being assigned. 
- Teacher will be able to change the attendance of the student only during that day. 
- If attendance of a student is not been marked it will be considered as absent at the end of the day.
- View for marking attendance should be a calender view. 

##  Student
- Student should be able to view his attendance as follow
  - Today's attendance
  - Weekly attendance
  - Monthly attendance
  - Total attendance percentage
  
 ## Report 
 - Sort students based on their attendance in the class. 
 - Student with highest attendance in each class.
 - Student with highest attendance in a school. 

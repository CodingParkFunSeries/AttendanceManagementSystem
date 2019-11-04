> # Attendance Management
> ### Access Levels: 
> Access will be given as authentication based on institute ID, which will be unique for each individual.
> * Full Read Full Write Access
> * Full Read Partial Write Access
> * Partial Read No Write Access
> ### User levels: 
> * Alpha Access: Admin here
> * Beta Access: Teachers in this case
> * Gamma Access: Students
> Assumptions: For the purpose of the project, it is assumed that attendance is marked manually: Teachers' attendance is marked by the admin,
> and the students', by the teachers.
> ### User Categories: 
> * **Admin** : Full read and write access, for all attendances, students and teachers.
> * **Teacher** : Partial write access: to students. Full read access
> * **Student** : Partial read access. Can read attendance, no write access.
> ## Procedure for attendance:
> * Admin manually marks attendance of teachers.
> * Teachers manually mark attendance of students.
> * It is assumed that although admin can mark presence of students, they do not normally do so. This is used only in circumstances described in [1]
> ### Algorithm for attendance: 
> * For Alpha to Beta: 
    ```C
    Beta[Given Date][Given Beta ID] = AttCount++
    ```
> * For Beta to Gamma:
    Gamma[Given Date][Given Gamma ID] = AttCount++
> * For Alpha to Gamma(Approved Leaves(see [1])):
    Gamma[Given approved date][Given Gamma ID] = AttCount++
    

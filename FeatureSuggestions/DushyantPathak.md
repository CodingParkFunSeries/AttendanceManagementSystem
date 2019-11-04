> # Attendance Management
> ### Access Levels: 
> Access will be given as authentication based on institute ID, which will be unique for each individual.
> * Full Read Full Write Access: Can read and update teachers' and students' data.
> * Full Read Partial Write Access: Can read teachers' data, can update students'.
> * Partial Read No Write Access : Can only read students' data.
****
> ### User levels: 
> * Alpha Access: Admin here
> * Beta Access: Teachers in this case
> * Gamma Access: Students
> ### Assumption: 
> For the purpose of the project, it is assumed that attendance is marked manually: Teachers' attendance is marked by the admin,
> and the students', by the teachers.
****
> ### User Categories: 
> * **Admin** : Full read and write access, for all attendances, students and teachers.
> * **Teacher** : Partial write access: to students. Full read access
> * **Student** : Partial read access. Can read attendance, no write access.
**** 
> ### Procedure for attendance:
> * Admin manually marks attendance of teachers.
> * Teachers manually mark attendance of students.
> * It is assumed that although admin can mark presence of students, they do not normally do so. This is used only in circumstances described in [1]
****
> ### Algorithm for attendance: 
> * For Alpha to Beta: 
>    ```
>    Beta[Given Date][Given Beta ID] = AttCount++
>    ```
> * For Beta to Gamma:
>    ```
>    Gamma[Given Date][Given Gamma ID] = AttCount++
>    ```
> * For Alpha to Gamma(Approved Leaves(see [1])):
>    ```
>    Gamma[Given approved date][Given Gamma ID] = AttCount++
>    ```
****
> ### Special Condition[1]
> In some special cases, attendance can be marked for students, even though they were not present, on accounts of
> * Representing the institute
> * Medical Leave
> * Emrrgency situations
> In such cases, the Admin(Alpha Access) will mark the date on which the students request attendance. The teachers will have no role in marking attendance on special circumstances.
****
> ### Additional Features: 
> * Some students also play the role of Teaching Assistant(TA). They have the right to mark students' presence. Hence, these particular students may be given Beta Access by Admin.
> * Statistics can be viewed individually by the students.
> * Teachers can view students' statistics individually, as well as grouped by date, and department, but they cannot view the statistics of any course they are not teaching. 
> Such permission, if required, will be granted by the admin.

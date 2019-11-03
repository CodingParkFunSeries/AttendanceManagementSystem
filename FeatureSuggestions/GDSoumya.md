# Attendance Management System

## Roles :
The system will have different levels of administration, the basic hierarchy could be followed :
1. Admin : All read/write permissions of system.
2. Support : Write access to only specific portions of data like user data for updating user details etc.
3. Manager : Read access to fetch all the attendance data.
4. User : Read permission for self data only.

All support amd manager accounts can only be created by the admin. The Admin account will be manually configured when the system is initialized for the first time.


## Basic Features

### 1. Register User :
A user must be registered and stored in DB before he can be logged into the AMS. The registration will have features specific to the type of AMS needed eg. Biometric, ID or Facial Recognition as required.

### 2. User Attendance :
User’s will be marked as present with their time of entry on a particular day only after they clear the authentication process which could be either through ID, biometric or facial recognition. At the end of the day all unmarked users will be marked absent.

### 3. Fetch Attendance :
The attendance of all users can be fetched in different possible ways as needed :
User Based : Attendance details of a specific user over a period of time.
Overall Attendance : Day wise attendance showing present users or absent users, over a period of time or specific date.
 
## Extra Features :

### 1. User Grouping :
In an organization the users can be grouped and sub-grouped depending on their designation and work. Each group will have their own Manager accounts which will only be able to fetch attendance details for that particular group only. The hierarchy can be extended further to group multiple groups under another group having a higher level Manager.

### 2. Weekly Attendance Notification :
All users will be sent their weekly attendance status.

### 3. Automated Warning :
If attendance of a user drops below a specific threshold a warning notification will be sent to the user.


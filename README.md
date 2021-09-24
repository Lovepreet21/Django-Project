# Django-Project
UMS
this project has django version 3.2.7 with postgreSQL 13.2, In order to run this project one need to add some data in few of the tables -> 
table1 -> Menu 
=> [Add 2 Menu with following details -> 
1. Menu Name: System Configuration, icon: fas fa-cog, link:/all_user_details/, submenu:True, priority:1, sm_priority:1, submenu_name:User Details] 

2. [Menu name: Department & Section, 'link:/faculty_dept_sec_detail/, icon:fas fa-university, priority:2, access_label:teacher]

Table2 -> Group -> Create 2 Groups:
 1. teacher
 2. student

Table3 -> Departments -> Add Few Departments
1. Computer Science & Engineering
2. Electronics & Electrical Engineering
3. Mechanical Engineering

Table4 -> Section -> Map Department With Section
1.  Computer Science & Engineering -> CSE001
2.  Computer Science & Engineering -> CSE002
3.  Computer Science & Engineering -> CSE003
1.  Electronics & Electrical Engineering -> MEC001
2.  Electronics & Electrical Engineering -> MEC002

After adding the entries create superuser account and login with superuser.

Access label field in Menu table is responsible for providing access to menu based upon the django group/role.
If the access_label field in menu table is empty then that menu is only accessible to superadmin.
if access_label field has value 'teacher' or 'student' then it is accessible to only 'teacher' or 'student' respectively.

After logging with super admin go to User Details Menu under System Configurtion Menu and 
Create New User by clicking on a +User button on the right hand side.

User with teacher role can also add the student in the application.

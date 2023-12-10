# ProjectJSP2
Read me before running the code, unzip the project file:
there is a clear versiom in Readme.docx!
Before, open the web application project in NetBeans IDE
First, Apache NetBeans IDE is required to perform the web application in java using html and jsp. (assume Apache NetBeans IDE is being installed)
You have to download the apache tomcat server zip files  https://tomcat.apache.org/download-10.cgi as default server connected with jsp files 
Download Mysql community server( depends on your computer version) and sql connector(.jar) in miscrosoft.com to perform mysql database.
https://dev.mysql.com/downloads/mysql/
https://dev.mysql.com/downloads/connector/j/5.1.html
After successful download, you have to initialize the mysql as below:
step1:. Start MySQL server
-       Open a command prompt
-       Go to the “bin” directory within the extracted root folder of the MySQL server with command “cd”
o   E.g., “cd C:\Users\student\Desktop\mysql-8.0.18-winx64\bin”
.   Initialization of the data directory with command
mysqld --initialize-insecure

-       Start the MySQL server with command
mysqld

 step2:. Execute SQL command to create user
-       Open another command prompt
.      Again, change to the “bin” directory of the extracted root folder of the MySQL server with command “cd”
-       a. Start the MySQL client as the “root”
mysql -u root

-       b. Create a new user called “mysqluser” with password “mypass”
create user 'user1'@'localhost' identified by '12345678';

-       c. Grant all privileges to the user for allowing the user to work on all databases
grant all privileges on *.* to 'user1'@'localhost' with grant option;

-       d. Logoff mysql with command
quit



mysql -u mysqluser -p

o   Note
§  The system will ask you for the password (i.e., “12345678”)

-       b. Create a database called “user” with command
create database user;

-       c. Use the database 
use user;


step3:Insert mysql commands from projectjsp.txt to create tables
1.login
2.student
3.studentcourse
4.teacher
5.admin
6.personal



step:4.Quit mysql
quit


Then, open the web application project in NetBeans IDE

Make sure the web application is runnable on your localhost server:

Select Apache Tomcat or TomEE and add your downloaded apache tomcat files which are stored in your computer. 
Then click next…
It will require you to set the username and password in everytime you re-opened and run the project files.
example:
username: admin
password: admin


Make sure click on the properties of project ( we named ProjectJSP)
to select libraries to add jar/folder that your download mysql connector jar with mysql

Select RUN in the below, to check your server information is matched, and choose a suitable default browser.

Then, run the codes in the project files.
Ensure you type in the url that is matched with the name of jsp files
for example, localhost:8080/ProjectJSP/login.jsp


REMARKS: 
The main code is located in the web page in the ProjectJSP
The user interface shown above is using macOS/iOS platform

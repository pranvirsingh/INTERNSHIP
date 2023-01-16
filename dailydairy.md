# 👉 Daily Dairy (12/07/22)
Download Ubuntu 22.04v linux operating system from Ubuntu official website. Make bootable drive of Ubuntu desktop using a tool [VENTOY](https://www.ventoy.net) and then Install in my laptop. Install some needy applications for linux like vscode, vim, etc. Also Learn how to use vim editor(little bit).

# 👉 Daily Dairy (13/07/22)
## Installing LAMP in Arch Linux

### Steps for the installation of LAMP are :-
- Installing Apache-web-server
    * Installing the Apache-web-server by using this command. ```sudo pacman -S apache``` in the terminal.
Install PHP dynamic server-side scripting language and its Apache module. 
    * ```sudo pacman -S php php-apache```
On the last step install MySQL database, choose 1 (MariaDB) community database fork then start and check daemon status.
    * ```sudo pacman -S mysql```
Now **LAMP** is installed in my system.

### Steps to secure MySql database

- The next step is to secure MySQL database by setting a password for root account, remove anonymous users accounts, remove test database and disallow remote login for user root.
    * ```sudo mysql_secure_installation```
Verify MySQL database connectivity by running the following command then leave database shell with quit or exit statement.
    * ```mysql -u root -p```

- Then I install php using this command.
    * ```sudo apt install php libapache2-mod-php php-mysql```


---

# 👉 Daily Dairy (14/07/22)
- Read about the frappe framework from [link](https://www.frappeframework.com) , its functionalities and advantages along with its installation. Also read about Jinja2 framework for templates.

---

# 👉 Daily Dairy (15/07/22)
- Install frappe framework using this [link](https://github.com/D-codE-Hub/Guide-to-Install-Frappe-ERPNext-in-Ubuntu-22.04-LTS) and face some problems and errors. I got an error in ```sudo mysql_secure_installation``` command and resolve this by searching on google.

---

# 👉 Daily Dairy (18/07/22)
- Make an app **library_management** using command ```bench new-app <app-name>``` using this [tutorial](https://frappeframework.com/docs/v13/user/en/tutorial/create-an-app)
- Then create a site **library5.test** using command ```bench new-site <site-name>``` following this [link](https://frappeframework.com/docs/v13/user/en/tutorial/create-a-site)
- Then install app on siteby using command ```bench --site library5.test install-app library_management```
- To confirm if the app was installed, run the command ```bench --site library.test list-apps```

---

# 👉 Daily Dairy (19/07/22)
- Create a DocType which is analogous to a Model in other frameworks. Apart from defining properties, it also defines the behavior of the Model. And before creating DocTypes, we have to enter developer mode by using this command ```bench set-config -g developer_mode true``` and then start our bench server.
- First I create a DocType named Article. To create it, click new then:
   * Enter Name as Article
   * Select Library Management in Module
   * Add the following fields in the Fields table:
      * Article Name (Data, Mandatory)
      * Image (Attach Image)
      * Author (Data)
      * Description (Text Editor)
      * ISBN (Data)
      * Status (Select) - Enter two options: Issued and Available (Type Issued, hit enter, then type Available)
      * Publisher (Data)

- Add some more features to DocType like Naming, Form Layouts and Permissions. Also add controllers methods which allow you to write business logic during the lifecycle of a document. 
- Create second DocType called **Library Member**. It will have the following fields:
   * First Name (Data, Mandatory)
   * Last Name (Data)
   * Full Name (Data, Read Only)
   * Email Address (Data)
   * Phone (Data)

---

# 👉 Daily Dairy (20/07/22)
- Create third DocType called **Library Membership**. It will have the following fields:
   * Library Member (Link, Mandatory)
   * Full Name (Data, Read Only)
   * From Date (Date)
   * To Date (Date)
   * Paid (Check)

- Create fourth DocType called **Library Transaction**. It will have the following fields:
   * Article - Link to Article
   * Library Member - Link to Library Member
   * Type - Select with 2 options: Issue and Return
   * Date - Date of Transaction

- Create last DocType called **Library Setting**. It will have the following fields:
   * Article - Link to Article
   * Library Member - Link to Library Member
   * Type - Select with 2 options: Issue and Return
   * Date - Date of Transaction

and follow the instructions given in the [frappeframework](https://www.frappeframework.com) website.

---

# 👉 Daily Dairy (21/07/22)
- Recreate the **Library Management System** website and study deeply the documentation of frappe framework.
- Complete Library Management System in Frappe using FrappeFramework Tutorial. Reference:[FrappeFramework](https://www.frappeframework.com)


:arrow_right: **Date : 22-JULY-2022** 

- Today our task is to create library management system in our laptop by learning through the frappe documentation https://frappeframework.com/
- In the library Management System we have to do the following things:-

We will build a simple Library Management System in which the Librarian can log in and manage Articles and Memberships. We will build the following models:

- Article: A Book or similar item that can be rented.
- Library Member: A user who is subscribed to a membership.
- Library Transaction: An Issue or Return of an article.
- Library Membership: A document that represents an active membership of a Library Member.
- Library Settings: Settings that define values like Loan Period and the maximum number of articles that can be issued at a time.

:arrow_right: **Date : 23-JULY-2022** 

### Saturday

:arrow_right: **Date : 24-JULY-2022** 

### Sunday

:arrow_right: **Date : 25-JULY-2022** 

- Today I learn how we can create our site and app in frappe folder:-
- Commands which use to create app is
```
bench new-app {app_name}
```
- For creating new site
```
bench new-site {site_name}
```
### Today I complete the following steps of Library Management System:-

- Frappe Framework Tutorial
- Install and Setup Bench
- Create an App
- Create a Site
- Create a DocType
- DocType Features

:arrow_right: **Date : 26-JULY-2022** 

### Today I completed the pending steps of library management system

- Controller Methods
- Types of DocType
- Form Scripts
- Web View Pages
- Today I complete the library management system and decide to give the presentation on it.

# :arrow_right: Date:(28-08-2022)
- Today Satinder sir assign a moodle task to my team(Jasjit,Komalpreet,Ranvir).The task was that we have to make a query in mysql to get the grade report of the user in moodle corresponding to their course.

# :arrow_right: Date:(29-08-2022)
- To complete the task (grade report),firstly i install local moodle on my system and it take some time.Then i start working on it and explore the feature of it ,because it was my first time to do something on moodle.

# :arrow_right: Daily-Work(30-08-2022)
- As i mention that i, installed the moodle on my system last day what today when i start working on it it show the error like (403 Forbidden)then  my friend Pranvir help me in this and tell me the solution tahat i have to stop the nginx.service and restart the  apache2.service.and it really solve my problem,thanku pranvir for your help. So we start our work on moodle grade report.

# :arrow_right: Daily-Work (1-09-22)
- Today @HS Rai sir give one task to me that we have to do some work on QT(Qt is cross-platform software for creating graphical user interfaces as well as cross-platform applications that run on various software and hardware platforms such as Linux, Windows). The first we have to learn about the QT how to use it and how it work. For this i install it in my system and start exploring about it.Then we install QT creator in which we write our program to create the GUI.Qt Creator creates several files for you. The HelloWorld.qmlproject file is the project file, where the relevant project configuration is stored. This file is managed by Qt Creator, so don’t edit it yourself. Another file, HelloWorld.qml, is our application code. Open it and try to understand what the application does before you read on.

# :arrow_right: Daily-Work (2-09-22)
- In this period we learn about the QT and run a simple program (Hello) on it.
- Beside this i am also workinfg on to get the user data from database.The question was that how to fetch the data from two table in mysql database.Because we have to fetch the user name and corresponding courses which are stored in two different tables.

# :arrow_right: Daily-Work (10-08-22)
- On this day sir give me new task of FET.FET(FET-6.7.5) is free software for automatically scheduling the timetable of a school, high-school or university. It uses a fast and efficient timetabling algorithm.

# :arrow_right: Dailt-Work (11-8-2022)
- Today i am also working on FET and tried to generate the timetable using random data.

# :arrow_right: Daily-Work (12-8-2022)
- Today I have successfully generate the time table and also shown to Rai sir but he told me that use `import` and `export` data commands and learn its documentation.

# :arrow_right: Daily-Work (13-8-2022)
- Listening all the presenation given by other GD members.

# :arrow_right: Daily-Work (15-8-2022)
- Learing about `import` and `export` commands. Rai sir given me one google sheet which contains the real data of civil department and told me that generates its timetable.

# :arrow_right: Daily-Work (16-8-2022)
- Today i have generated the civil department timetable then rai sir said me find that where all these files stored and where its source code is present.

# :arrow_right: Daily-Work (17-8-2022)
- Learing about `import` and `export` commands. Rai sir given me one google sheet which contains the real data of civil department and told me that generates its timetable.
- I have found that where source code is present and then rai sir said that also find now if once timetable is generated  after that we change some infomation in its csv files ,is it also reflect in generated timetable or not?
 
# :arrow_right: Daily-Work (18-8-2022)
- Today i have started working on rai sir task but after done all testing i have reached that thers is not reflect of modify information in generated timetable and wanted to modify then generate the same timetable again.

# :arrow_right: Dailt-Work (19-8-20222)
- Today was my task to enable the `Level-5` or `Level-7`. `Level-2` is by default set. 
- `Level-7` is used to highlight the words. Till evening i have enables it successfully.

# :arrow_right: Daily-Work (20-8-2022)
- Today's in morning Rai sir told me again now without using GUI of `FET` software generate the timetable. On the backend fet will run and takes the csv files (user will upload) and genearate the timetable in the backend and give the link of generated timetbale as a output.

# :arrow_right: Daily-Work (22-8-2022)
- Today Satinder sir given me work of moodle.I have to created a Courses cateogries there using CSV files of NSPS.

# :arrow_right: Daily-Work (23-8-2022)
- I have done one blunder mistake while creating the course categories which is told by satinder sir to me and said create the categories of courses again.

# :arrow_right: Daily-Work (24-8-2022)
- I have created all the courses again and also putt the subjects in each category.This task took complete one day.

# :arrow_right: Daily-Work (25-8-2022)
- Today Satinder sir given a task to me and jasjit to find the information from database regarding to the NSPS grade report. A grade report is contains the fields of `Name of course` , `Email address` , `Course grade` etc.

# :arrow_right: Daily-Work (26-8-2022)
- Today we learnt first about the sql queries and watched one tutorial for it and explore about the general log file and error log file along what is the importance over all of these files. After wacthed the tutorial got some idea and executed some queries.

# :arrow_right: Daily-Work (27-8-2022)
- Finally we took our first step towards the task. To complete the task (grade report),firstly i install local moodle on my system and it take some time.Then i started working on it and explore the feature of it ,because it was my first time to do something on moodle.

# :arrow_right: Daily-Work (29-8-2022)
- In order to accomplished our task ,we need user(student) name,grade,id,couse name.So start exploring the moodle database to get the valuses from the moodle database tables.
- `mdl_grade_grades`: In this table we get the id,rawgrademax,finalgrade.
- `mdl_user`: In this table we get the firstname of user,last name of user,username.
- `mdl_course`: In this we get id of course,fullname,shortname.

# :arrow_right: Daily-Work (30-8-2022)
- Today we had a discussion with our mentor releted the values and we set the final table ,to make single final query. The final table that we have to make contain the feild of uasername,firstname,lastname,course name,id.

# :arrow_right: Daily-Work (31-8-2022)
- We succesfilly make the query with the help of Satinder sir, and at last sir tell us to check the final output, is it was actually meet with our requirement. At that time it was correct but when we test it by adding more courses then it was not giving the update couse and update grade of user.

# :arrow_right: Daily-Work (1-9-2022)
- Today i had a task to resolve the problem. For that i took help from my other training friends. We all start working on it and also finding the solution with diffrent diffrent approaches.

# :arrow_right: Daily-Work (2-9-2022)
- Today i went to satinder sir to discuss the problem. Sir gave some idea about it we again start to working on it and applied several queries but didn't work anything till evening.

# :arrow_right: Daily-Work (3-9-2022)
- On this day i try below query-
`SELECT u.firstname , u.lastname , u.email , u.username, c.fullname as course_name,  
ROUND(gg.finalgrade,2) Grade, concat(uo.url, c.id) as url FROM mdl_course AS
c JOIN  url_of_course AS uo JOIN mdl_context AS ctx ON c.id = ctx.instanceid 
JOIN mdl_role_assignments AS ra ON ra.contextid = ctx.id JOIN mdl_user 
AS u ON u.id = ra.userid JOIN mdl_grade_grades AS gg ON gg.userid = u.id JOIN 
mdl_grade_items AS gi ON gi.id = gg.itemid JOIN mdl_course_categories 
AS cc ON cc.id = c.category WHERE gi.courseid = c.id AND gi.itemtype = 'course';`
- It executed successfully getting the final output which mathes with requirements.

# :arrow_right: Daily-Work (4-9-2022)
- After this having a task to put the incremental backup so that automatically values will be fetched from the database and update on moodle (gradebook) respectively.

# :arrow_right: Daily-Work (5-9-2022)
- Today i have a task to learnt about the incemental backup. For that i refers some tutorial from youtube and followed them. I learnt of its importance and significance.

# :arrow_right: Daily-Work (6-9-22)
- Today @HS Rai sir give one task to me that we have to do some work on QT(Qt is cross-platform software for creating graphical user interfaces as well as cross-platform applications that run on various software and hardware platforms such as Linux, Windows). The first we have to learn about the QT how to use it and how it work. For this i install it in my system and start exploring about it.

# :arrow_right: Daily-Work (7-9-22)
- Then we install QT creator in which we write our program to create the GUI.Qt Creator creates several files for you. The HelloWorld.qmlproject file is the project file, where the relevant project configuration is stored. This file is managed by Qt Creator, so don’t edit it yourself. Another file, HelloWorld.qml, is our application code. Open it and try to understand what the application does before you read on.

# :arrow_right: Daily-Work ((8-10)-09-22)
- In this period we learn about the QT and run a simple program (Hello) on it.
- Beside this i am also workinfg on to get the user data from database.The question was that how to fetch the data from two table in mysql database.Because we have to fetch the user name and corresponding courses which are stored in two different tables.

# ➡️ght: Daily-Work (14-9-22)
- Today We start a ndew Project named CMC( Construction & Maintenance Cell).First of all we need to understand the structure of CMC, The CMC will be a company under NSET, parallel to GNDEC. IMO it must be a service based company, what is your opinion, and other domains available.It will have sales, purchase, stock, accounting etc.So, It is a service based company.

# :arrow_right: Daily-Work (15-9-22)
- Create a company at gne2 and set its domain to service. We will test over gne2.But We have a maintenance module.Here we can make others doctype related to maintenance.So, the Company Name : Construction & Maintenance Cell, Parent Company : NSET, Domain Name : Services

# :arrow_right: Daily-Work (16-9-22)
- Create a dashboard for the maintenance request.
- In which cmc user see the requests by date wise and see no. of requests per day.

# :arrow_right: Daily-Work (17-9-22)
- In the web form, "justification for request"  field needs to be optional, not mandatory. And it needs to be "draft" upto the level of HoD, which means that HoD/OIc/Caretaker/Warden will be able to change it. No change will took place once the higher authority forwarded the request.

# :arrow_right: Daily-Work (18-9-22)
- Today, I am working on Dashboard. Start learning about the Dashboard and make test dashboard.Becauses ,I have to make a Dadboard of all Higher Authorities like SDO,CMC -Head, HOd's of all Departments.

# :arrow_right: Daily-Work (19-9-22)
- Today we are working on the workflow of CMC project. We made the flowchart of CMC Project.
- steps: student | employee -> HoD -> SDO -> O/Ic Incharge 
- But there migh be Student -> Caretaker -> Warden -> SDO or Lab Attendant | Lab Technician -> Lab Incharge -> HoD ... In case of rejected, all must see the status, and in case of any additional query it may be sent back from where is was forwarded.

# :arrow_right: Daily-Work (20-9-22)
- Today i work with Satinderpal sir , sir said us to make a courses on guru.gndec.ac.in.So we make it on the site.

# :arrow_right: Daily-Work (21-9-22)
- Solved the problem regarding the moodle like user are not enroll in the courses and their attebdance.

# :arrow_right: Daily-Work (22-9-22)
- Beside the CMC project I also work on the NSPS project(School project).Firstly we visit the school and get the information about the courses or subject and teacher or student data of school.

# :arrow_right: Daily-Work (23-9-22)
- According to the information we upload the courses and user in the gne1.gndec.ac.in which is official moodle site of School.

# :arrow_right: Daily-Work ((24-29)-9-22)
- Working on gne1.gndec.ac.in and visit the school regulary.Solves the teachers problems, help them to access the gne1.gndec.ac.in and how to add the activity in it and turm the edit mode on to do some work.

# :arrow_right: Daily-Work (30-9-22)
- Today we (I and Pranvir ) are going to implement stock items in
erp.gndec.ac.in and also creating a dashboard of SDE which is only
visible to SDE only.

# :arrow_right: Daily-Work (1-10-22)
- We are going to add stock items to erp.gndec.ac.in and make a
dashboard for SDE which is only visible to SDE.

# :arrow_right: Daily-Work (2-10-22)
- Today we have to fullfil the requirement that are pending that thses are disscussed with Rai sir.
- I changed the Nature of work according to the requirements.

# :arrow_right: Daily-Work (3-10-22)
- Estimate work is done on erp.gndec.ac.in according to the requirements.

# ➡️Daily-Work (4-10-22)
- I checked that if we select items for estimate then it will also reduces in stock.
- Now our task is to create a button in the CMC request form for SDE
only in which SDE will manage the realtime stock items.

# :arrow_right: Daily-Work (5-10-22)
- We have two options:
`First`:
- We can add a custom button in the cmc request form using the form
script. The link which is following is:
`https://frappeframework.com/docs/v13/user/en/api/form`
- But here we have an issue of permissions. Because Custom button is
not a field in a doctype and in my knowledge we are only able to gives
permissions to doctype fields to show that fields to some specific
users so here we goes to our Second option
`Second`:
- We can create a field which is of type "Button". I know this is a
silly question but how can we add links behind the Button type fields
in frappe??
- I searched this on Google and found that we need to write custom
scripts to make this button working. But I didn't get the correct
syntax for this.

# :arrow_right: Daily- Work (6-10-22)
- we checked that if we select items for estimate then it will also reduces in stock.So when our stock becomes completely empty then we need to send
quotations for required items. So now our next task is to send quotations and restore our stock again.

# :arrow_right: Daily-Work ((7-12)-10-22)
- Today Task was to do a Company Setup. So we are going to do the company setup.The company we are going to create  is Manufacturing company.
- Our Company name is "Unique Number Ltd" under Domain "Manufacturing".
- Company (Unique Number Ltb) is successfully created on gne2. Now we are going to do our next step.
- Our next step is to define tax of a company under the section of chart of account.
- In the section of Chart and Account , we select our company and come under the source of funds section . Here we do some changes in the CGST and SGST according to requirements which come under the Duties and Taxes.
- We created incoming CGST and incoming SGST under Application of assets section in the chart of accounts for buying purposes and defined CGST and SGST under Source of funds section for selling purpose.
- We need to create a journal entry to show the amount in the chart of accounts. But when we make a general entry it shows the error which says set the fiscal year first.
- In this we firstly add the sales order which include the information
about the customer,item and delivery date.
- Sales Invoice done.Payment of this order is also done

# :arrow_right: Daily-Work (13-10-22)
- Dashboard for principal is created on erp.gndec.ac.in
- After this we disscuss the project with sir and there many thing which are need to be add in the project like.

# :arrow_right: Daily-Work (14-10-22)
- "new request" button in cmc request.
- Item name in estimate automatically fetched.
- These tasks have been completed.

# :arrow_right: Daily-Work (15-10-22)
- sorting complaint number in my requests
- Tasks is completed.

# :arrow_right: Daily-Work (16-10-22)
- We (Me and Komalpreet) are going to make new departments which are
left and will also update the csv file accordingly and upload it in
erp.gndec.ac.in.

# :arrow_right: Daily-Work (17-10-22)
- Employees also created successfully.On erp.gndec.ac.in
- Task was completed: Image size limit can change as we tested on gne2.gndec.ac.in.
It can be changed through the backend. To change the image size limit,
go to /sites and open "common_site_config.json".
change max_file_size: 500000.

# :arrow_right:Daily-Work (18-10-22)
- Working on Home page.
- I add a nav bar.(About, Departments, Notice board, Faculties).

# :arrow_right: Daily-Work (19-10-22)
- Working on Education Domain . 
- I work on education domain t done the project regarding the Student Enrollment.
- Firstly under stand the whole process and had meeting with sir.

# :arrow_right: Daily-Work (20-10-22)
- Understand the Fee structure  in Edcation Domain.
- Student Enrollment Process.

# :arrow_right: Daily-Work ((21-30)-10-22)
- Create ourses in the education domain.
- Create Fee structure (Fee component, Student Category, Program)
- Add student and instructor in the list.

# :arrow_right: Daily-Work ( 1-11-22)
- Rai sir told us to replace the estimate by quotation.
- Our approach is that we are going to create a button named "quotation
estimate" which will be shown to the SDE. With the help of this
button, SDE will be able to handle quotations(estimate), sales order,
sales invoice(Bill).

# :arrow_right: Daily- Work (2-11-22)
- We successfully created a quotation. Now we are going to create a
sales order of that quotations, in which we add our items which we
want. And here we also apply a Tax on items, discounts and on them.

# :arrow_right: Daily-Work (3-11-22)
- we can update the quotation values in the estimate table.For this sdo willlick on a button named "Quotation/Estimate" in the cmc requestform and redirect to the quotation form. And then the estimate table values will be autofetch from the quotation table.

# :arrow_right: Daily-Work (4-11-22)
- We created 2 Doctypes named:
- final testing
- DemoQuotation2
- We added the same child table "estimate duplicate" in both doctypes as
- We mentioned above. But according to that we didn't get the results.

# :arrow_right: Daily-Work (5-11-22)
- Make a new flowchart of CMC Estimate/Quotations according to
@Satinder sir idea .

# :arrow_right: Daily- Work ((6-13)-11-22)
- FullFil the requirents and do some changes in the fee structure and did some work on dashboard like add some filters in the cards and chardts of dashboard.

# :arrow_right: Daily-work (14-11-22)
- Today my task was to complete the requirements of CMC Project.The requirements  that we have to fullfile are:
- If sales invoice value exceeds estimated cost then give alert message.
- If sales invoice value exceeds Sanctioned cost then shouldn't generate the bill.
- Inorder to complete we think that these requirements may be completed by the
  Notification feature in frappe. Me and pranvir just check it and we
  see that we can apply the condition in the "Condition" field. But this does not work for us.
- Then we find one more solution that, there is a feature in client script called frappe.msgprint(). This function can be used with some conditions, so we can apply our conditions here.
- Firstly we follow this link https://discuss.erpnext.com/t/client-script-to-fetch-value-from-another-doctype/1095/3 tutorial, to get alert message in sales invoice. In this tutorial we use one script and we test it on **gne12.gndec.ac.in**.

# :arrow_right: Daily-Work (15-11-22)
- Before start work things that i learn are :
- Connection in doctype:
Inorder to make connection we have to link two filed in both doctype and the link field take the data from the linked doctype.

# :arrow_right: Daily-Work (17-11-22)
- In the morning, I learn from my team member that how we can apply condition  in the doctype ,like we have to do one task that get the alert message when total bill(sales invoice) is greater then the estimate cost. 
- I do discussion with team about student data or informtion because we have to add the hosteler(student) in the CMC project.So just create 5,6 student then enroll them in their respective program(CSE,MBA etc) and course(subject).This work com eunder the Education Domain in the erp.
- In the afternoon there was a meeting with teachers(Mentors) about our task and guidlines.In the meting we put our points and did the discussion about the project.
- Now my task was to upload the user(employee)on erp.So this work is done through Data import list ,where i  download the template according to requirment and put the provided data in the downloaded template and save it with .csv extenstion.There was  many  problem faced by me while uploading the user which are:
1) In the first time it showing the error that **The following values do not exist for Department: Computer Science Engineering – GNDEC**
2) Error regarding the User id of user(employee) which was their e-mail.

# :arrow_right: Daily-Work (18-11-22)
- Today at morning 8:30 uploading the left user on erp.gndec.ac.in
- 9:00 Disscuss the CMC project with team.
- 10:25 Disscuss the Nankana Project with Satinder sir and had a meeting with Nankana School officals at 11:15.
- 11:15-12:26 In the meeeting we show our work to them and get their views on it and their requirements.
- 12:38 Discuss a problem related to the guru.gndec.ac.in with Amarpreet Mam(MBA Block).
- Working on rest of work.
  
# :arrow_right: Daily-Work (19-11-22)
- Today we went to the Nankana School and had the meeting with teachers .In the meeting they show us their feebank software and school fee structure.
- In the evening their was seminer of other GD members .

# :arrow_right: Daily-Work (21-11-22)
- Start working on Nankana Public school project and trying to meet their requirements in student applicant form.
- 10:32 -  The first thing they want in sibling  details  table is that
they only want to select the student ID and other details of selected
student come accordingly.This  work is done , now we only have to select the
student id and corresponding to this  First ,last name ,gender and
date of birth is come accordingly.
- Set the stock problem in erp.gndec.ac.in ,like disable the unwanted item .
- Trying to solve the error in quotion , like it was give the error of multicurrency _ invoice while creating the sales invoice.

# :arrow_right: Daily-Work (22-11-22)
- Working on Education domain like Student Admission ,Fees.
- Did some work on guru.gndec.ac.in, solved the problems faced by teacher regarding participents in the courses.
  
# :arrow_right: Daily-Work (23-11-22)
- Today i make connection of fee on student applicant form.
- Work on Fees Structure and make some program and fee category.

# :arrow_right: Daily-Work (24-11-22)
- Make some LDAP user then upload and enroll them in their respective courses.
- Make duplicate of student applicant form to do same changes without changing the core of form.
- Make refrence workflow to understand the process and discuss it with Komal.

# :arrow_right: Daily-Work (25-11-22)
- Today , I work on Nanak School project :
- Create the doctype Applicant Form ,add the connection of Applicant
fee in the doctype.
- Did some work on a CMC project like Company address and learned one thing that we can we a customer an internal customer under representing company from @ Rai sir.
- Create one more doctype Registration Form and also add the connection  form where Applicants who submit the applicant fee can submit his/her registration fee (5000).
- Things now i am going to do is that in the registration fee form ,fee component fetch automatically while selecting the fee structure.

# :arrow_right: Daily-Work (26-11-22)
- Today ,I am going to set the  view of the dashboard for the accountantmam(Nankana School Teacher). After this i will work on fee structure and fee         concession according to the school.

# :arrow_right: Daily-Work (28-11-22)
- This morning all SDC members had a meeting  (google meet) with Satinder Sir regarding work progress . So in the meeting we discussed our problem  and    work status with sir.In our task (School project), sir told us to make workflow for applicant and registration forms instead of making different doctype
for each stage. Set permissions under it until the applicant did not deposit 500/- could not be able to open the registration form. Similarly if    registration has been completed only then he/she is able to see the enrollments.
So, now we(Jasjit, Komalpreet) are working on it .

# :arrow_right: Daily-Work (29-11-22)
- Today we had a discussion with @ Satinderpal Sir and sir told us that we have to do all the steps (applicant and registration fee )  in one
doctype.For this we have to make three connections (Applicant fee , Advance Fee or Registration fee , Admission fee) in one doctype so it will be easy for us to do all the steps accordingly.
- I made one doctype named Student Form in gne12 and added the three connections of fees which are shown after saving the form. These fees are Applicant Fee , Advanced Fee and Fee.

# :arrow_right: Daily-Work (30-11-22)
- Today my task is to add an Action button of Approved , Reject and
Enroll button on student applicant doctype so that after submitting
the fees and applicant form we enroll the applicant in a program or
course.

# :arrow_right: Daily-Work (1-12-22)
- Last we discuss the Student Applicant process with @ Satinderpal Sir and sir said us to make the connection of fees on one doctype so accordingly to sir we create one doctype named Waheguru on gne2.gndec.ac.in under Education Domain . In this doctype we (me, Komalpreet) make the connection of Applicant fee, Advanced Fee.After saving the form these connections are visible  and then we submit the form.
Then the task was to add an action button on this, this action button was about Approved or reject the form and after applying the condition of approved or reject we update the form the enroll option to enroll the applicant in the Program.
- Now the problem we faced was that when we enroll the applicant by clicking on Enroll button on Waheguru doctype it shows that:
"Student Applicant NSPS-SESSION-2023-2024-00003 not found" So, we are going to resolve the conflict.
- I think that it is because there is no relation between Waheguru and Program Enrollment doctypes , so now I am going to see it and report here regularly if it work.

 # :arrow_right: Daily-Work (2-12-22)
 - Today we crete the user for NSPS school. These user are the Teachers ,so give them Instructor role at last. The main motive was  to show the courses to the instructor. For this we have to create the program ,courses. 
 
 # :arrow_right: Daily-Work (3-12-22)
 - Today we had a discussion with @Satinderpal Sir regarding completing
the Nankana Sahib Public School project. So, Satinderpal Sir told
us(Jasjit Kaur and Pranvir SIngh) to complete this project as soon as
possible.
- Our first requirement is to submit the applicant form of the student
applicant. So, in gne2.gndec.ac.in, we customize a student applicant
doctype which fulfill our requirement. We also make a connections of
applicant fee(500) which is shown after save the form of student
applicant. Here is the link:
https://gne2.gndec.ac.in/app/student-applicant/new-student-applicant-1

# :arrow_right: Daily-Work (4-12-22)
 Sunday
 
 # :arrow_right: Daily-Work (5-12-22)
 - Now our task is to check the ledger of the applicant fees.
 - To check the ledger, we create an action button named "View" in a
doctype. Through this button, we can see the accounting ledger. But
the Problem is that Ledger is shown but with 0 amount(credit and debit
value 0). Beside this, it does not show the Voucher No.

# :arrow_right: Daily-Work (6-12-22)
- After trying a lot, we found that this problem occurred due to the
party type.
- There are already predefined party types that are created
in erpnext. 
- But the Administrator has no permission to create a new
party type. We can resolve this problem by creating a new party type.

# :arrow_right: Daily-Work (7-12-22)
- In erp.gndec.ac.in:Predefined party types are:
1) Student
2) Shareholder
3) Employee
4) Supplier
5) Customer
- In our case, We need to create a student applicant not a student. So,
we need to create new party type of doctype "Student Applicant".

# :arrow_right: Daily-Work (8-12-22)
- This problem is solved now. 
- Early we thought that this problem occurs
because of the party type.But after adding more party type (student
applicant) problem is not solved.
- So we checked that this all is
because of the Company setup.

# :arrow_right: Daily-Work (9-12-22)
-  Initially we use the NSPS company and in
the ledger the account value is zero(0), but after using the SDC
company for the transaction the problem is solved .
- Now  in the ledger we see all the transections.

# ➡️ Daily-Work (10-12-22)
- As per the discussions, @Satinder sir and @Rai sir we come to the
point that for the moment we skip the student applicant process and
start working on "Lead".
- And we add a fee connection to show the
ledger of that party, which is showing correctly.

# ➡️ Daily-Work (11-12-22)
Sunday

# ➡️ Daily-Work (12-12-22)
- Firstly we tested it localy.
- gne12.gndec.ac.in the student applicant work is not working properly. 
- We give a demo.

# ➡️ Daily-Work (13-12-22)
- We discussed with @Satinder sir that students are also eligible to
submit the registration fees and applicant fees(500).
- For this, we firstly create a registration form, in which students fill their details regarding admission.
- So the next step is after submitting the registration form, students submit their respective fees.

# :arrow_right: Daily-Work (14-12-22)
- But actually we don't have any idea about this. How students can submit their fees online. 
- And we did this work locally. Now we are going to implement it on gne2.gndec.ac.in.
- In discussion with @Satinder sir, we came to the point that students can also submit their fees online but the doubt is at which mode they can submit their fees(like paytm, google pay, or many more methods).

# ➡️ Daily-Work (15-12-22)
- Rai sir give us idea about student online payment.
- "It depends on payment gateway. Once that is implemented, all supporter / selected methods will be available. "
- So we are start exporing it.Like what is payment gateway, their methods etc.

# ➡️ Daily-Work (16-12-22)
- Me and pranvir have made the form to collect the registration fees that is 500/- from the student.
- @ Raghav and @simran have attached the button to pay fee that would be link to the online razorpay gateway.
- Now  they are asking for the API key and API secret to make the razorpay working.

# ➡️ Daily-Work (17-12-22)
-  we are going to do our work on
gne2.gndec.ac.in:8002, so in this we create the Web form of
Registration Form but when after filling the details we are unable to
save the form while discard button is working but we don't know why
save button is not working.
- We check that all the existing webforms are submitting successfully if
we create a new webform then it doesn't.

# ➡️ Daily-Work (18-12-22)
Sunday

# ➡️ Daily-Work (19-12-22)
- In gne12.gndec.ac.in we have inbuilt Razorpay integration setting in
the "Integrations" section. 
- But in gne2.gndec.ac.in we don't have a razorpay integration option.

# ➡️ Daily-Work (20-12-22)
- The solution is that we only have to add one doctype named "Razorpay
Settings".
- Under module "integrations" then we customize the workspace
of Integration page.

# ➡️ Daily-Work (21-12-22)
- Now sir fill the API key in gne2.
-  Now we create the webform which is filled by the student:
https://gne2.gndec.ac.in/registration/new
- In this webform, we create a button for Razorpay fees. Please check if
this is correct.

# ➡️ Daily-Work (22-12-22)
- To the moment we switch to the CMC project.
- In order to complete the CMC project @Satinder assigned this task to
one team(Pranvir, Jasjit, Sahilpreet). As per the discussion with
@satinder sir in the morning, sir said that we should have to test the
whole CMC Project in gne2.gndec.ac.in.

# ➡️ Daily-Work (23-12-22)
- So, now in the gne2.gndec.ac.in we are going to make a doctype of
Maintenance form and also webform of this form.
- first we will test it only for the employee. After this we will
move to the hosteler part.
- Doctype(Maintenance)  and Webform(Maintenance Form) is created on
gne2.gndec.ac.in. But at moment I didn't give any permission.

# ➡️ Daily-Work (24-12-22)
- Doctype(Maintenance)  and Webform(Maintenance Form) is created on
gne2.gndec.ac.in. But at moment I didn't give any permission.
- Beside this I am going to do a company setup in the gne2.gndec.ac.in
and under that company I will create the Departments.

# ➡️ Daily-Work (25-12-22)
Sunday

# ➡️ Daily-Work (26-12-22)
- Now we give some  Perm level permission to the specific field and
these permissions are also given to the SDE and CMC Head.
- Now our pending task for CMC is to keep and maintain the record of
warehouse items .
- There are many options
which are not explored by us.  Like after making the quotation we made
a sales order for that quotation, then we have many options like Pick
list and Delivery Notes etc for the corresponding Sales order.

# ➡️ Daily-Work (27-12-22)
- For the testing purpose we are going to make 2 test users in
erp.gndec.ac.in  to check the current process or status of the work.
- While testing we make the 2 hod test user
(1.CSE, 2.IT).So I sent one maintenance request from an employee of
the CSE department but found that this request was shown to the HOD of
the IT department also. We now we are working on it.
- According to us, Department wise workflow is not working properly
because of this we face this problem.

# ➡️ Daily-Work (28-12-22)
- To the solution we find that  we did not give them Department permission in Set User Permission.
- Check under user permission whether the HoD has permission of
corresponding department, if there is not such permission, add new
with allowing the department for value of respective department.
-  now it is working.

# ➡️ Daily-Work (29-12-22)
- The things that we notice are that items in the stock are not as per
requirements like we are facing the problem regarding item price of
the item. Beside this there is a problem regarding the Sanctioned cost.
- Sanctioned cost will only be visible to SDE after CMC Head approved
that request and fill sanctioned cost. But, it is not working like
that. It is the problem of permission levels. So, now we are working
on it.

# Daily-Work (30-12-22)
- While doing the transactions between the parties we found that there
is no implementation of Razorpay Settings in erp.gndec.ac.in.
- Now we are just trying to pay the bill using the link "payment" in a
direct way. According to that, we need a bank account for the customer
party. So, now we are making a dummy bank account for GNDEC(Company).

# ➡️ Daily-Work (1-01-23)
New Year and Sunday


 








 
 








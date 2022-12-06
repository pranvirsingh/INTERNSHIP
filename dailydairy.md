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








# Daily-Work (14-9-22)

- Today We start a ndew Project named CMC( Construction & Maintenance Cell).First of all we need to understand the structure of CMC, The CMC will be a company under NSET, parallel to GNDEC. IMO it must be a service based company, what is your opinion, and other domains available.It will have sales, purchase, stock, accounting etc.So, It is a service based company.

# Daily-Work (15-9-22)

- Create a company at gne2 and set its domain to service. We will test over gne2.But We have a maintenance module.Here we can make others doctype related to maintenance.So, the Company Name : Construction & Maintenance Cell, Parent Company : NSET, Domain Name : Services

# Daily-Work (16-9-22)

- Create a dashboard for the maintenance request.
In which cmc user see the requests by date wise and see no. of requests per day.

# Daily-Work (17-9-22)

- In the web form, "justification for request"  field needs to be optional, not mandatory. And it needs to be "draft" upto the level of HoD, which means that HoD/OIc/Caretaker/Warden will be able to change it. No change will took place once the higher authority forwarded the request.

# Daily-Work (18-9-22)

- Today, I am working on Dashboard. Start learning about the Dashboard and make test dashboard.Becauses ,I have to make a Dadboard of all Higher Authorities like SDO,CMC -Head, HOd's of all Departments.

# Daily-Work (19-9-22)

- Today we are working on the workflow of CMC project. We made the flowchart of CMC Project.
- steps: student | employee -> HoD -> SDO -> O/Ic Incharge 
- But there migh be Student -> Caretaker -> Warden -> SDO or Lab Attendant | Lab Technician -> Lab Incharge -> HoD ... In case of rejected, all must see the status, and in case of any additional query it may be sent back from where is was forwarded.

# Daily-Work (20-9-22)

- Today i work with Satinderpal sir , sir said us to make a courses on guru.gndec.ac.in.So we make it on the site.

# Daily-Work (21-9-22)

- Solved the problem regarding the moodle like user are not enroll in the courses and their attebdance.

# Daily-Work (22-9-22)

- Beside the CMC project I also work on the NSPS project(School project).Firstly we visit the school and get the information about the courses or subject and teacher or student data of school.

# Daily-Work (23-9-22)

- According to the information we upload the courses and user in the gne1.gndec.ac.in which is official moodle site of School.

# Daily-Work ((24-29)-9-22)

- Working on gne1.gndec.ac.in and visit the school regulary.Solves the teachers problems, help them to access the gne1.gndec.ac.in and how to add the activity in it and turm the edit mode on to do some work.

# Daily-Work (30-9-22)

- Today we (I and Pranvir ) are going to implement stock items in
erp.gndec.ac.in and also creating a dashboard of SDE which is only
visible to SDE only.

# Daily-Work (1-10-22)

- We are going to add stock items to erp.gndec.ac.in and make a
dashboard for SDE which is only visible to SDE.

# Daily-Work (2-10-22)

- Today we have to fullfil the requirement that are pending that thses are disscussed with Rai sir.
- I changed the Nature of work according to the requirements.

# Daily-Work (3-10-22)

- Estimate work is done on erp.gndec.ac.in according to the requirements.

# Daily-Work (4-10-22)

- Me checked if we select items for estimate then it will also reduces in stock.
- Now our task is to create a button in the CMC request form for SDE
only in which SDE will manage the realtime stock items.

# Daily-Work (5-10-22)

- We have two options:
First:
We can add a custom button in the cmc request form using the form
script. The link which is following is:
https://frappeframework.com/docs/v13/user/en/api/form
 But here we have an issue of permissions. Because Custom button is
not a field in a doctype and in my knowledge we are only able to gives
permissions to doctype fields to show that fields to some specific
users so here we goes to our Second option

Second:
We can create a field which is of type "Button". I know this is a
silly question but how can we add links behind the Button type fields
in frappe??
I searched this on Google and found that we need to write custom
scripts to make this button working. But I didn't get the correct
syntax for this.

# Daily- Work (6-10-22)

- we checked that if we select items for estimate then it will also reduces in stock.So when our stock becomes completely empty then we need to send
quotations for required items. So now our next task is to send quotations and restore our stock again.

# Daily-Work ((7-12)-10-22)

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

# Daily-Work (13-10-22)

- Dashboard for principal is created on erp.gndec.ac.in
- After this we disscuss the project with sir and there many thing which are need to be add in the project like.

# Daily-Work (14-10-22)
 
 1) "new request" button in cmc request.
 7) item name in estimate automatically fetched.
 - these tasks have been completed.

# Daily-Work (15-10-22)

 2) sorting complaint number in my requests
 - Tasks is completed.

# Daily-Work (16-10-22)

- We (Me and Komalpreet) are going to make new departments which are
left and will also update the csv file accordingly and upload it in
erp.gndec.ac.in.

# Daily-Work (17-10-22)

- Employees also created successfully.On erp.gndec.ac.in
- Task was completed: Image size limit can change as we tested on gne2.gndec.ac.in.
It can be changed through the backend. To change the image size limit,
go to /sites and open "common_site_config.json".
change max_file_size: 500000.

# Daily-Work (18-10-22)

- Working on Home page.
1)  I add a nav bar.(About, Departments, Notice board, Faculties).

# Daily-Work (19-10-22)

- Working on Education Domain . 
- I work on education domain t done the project regarding the Student Enrollment.
- Firstly under stand the whole process and had meeting with sir.

# Daily-Work (20-10-22)

- Understand the Fee structure  in Edcation Domain.
- Student Enrollment Process.

# Daily-Work ((21-30)-10-22)

- Create ourses in the education domain.
- Create Fee structure (Fee component, Student Category, Program)
- Add student and instructor in the list.

# Daily-Work ( 1-11-22)

- Rai sir told us to replace the estimate by quotation.
- Our approach is that we are going to create a button named "quotation
estimate" which will be shown to the SDE. With the help of this
button, SDE will be able to handle quotations(estimate), sales order,
sales invoice(Bill).

# Daily- Work (2-11-22)

- We successfully created a quotation. Now we are going to create a
sales order of that quotations, in which we add our items which we
want. And here we also apply a Tax on items, discounts and on them.

# Daily-Work (3-11-22)

-  we can update the quotation values in the estimate table.For this sdo willlick on a button named "Quotation/Estimate" in the cmc requestform and redirect to the quotation form. And then the estimate table values will be autofetch from the quotation table.

# Daily-Work (4-11-22)

- We created 2 Doctypes named:
1) final testing
2) DemoQuotation2

We added the same child table "estimate duplicate" in both doctypes as
we mentioned above. But according to that we didn't get the results.

# Daily-Work (5-11-22)

- Make a new flowchart of CMC Estimate/Quotations according to
@Satinder sir idea .

# Daily- Work ((6-13)-11-22)

- FullFil the requirents and do some changes in the fee structure and did some work on dashboard like add some filters in the cards and chardts of dashboard.

# Daily-work (14-11-22)
Today my task was to complete the requirements of CMC Project.The requirements  that we have to fullfile are:

1) If sales invoice value exceeds estimated cost then give alert message.

2) if sales invoice value exceeds Sanctioned cost then shouldn't
generate the bill.

- Inorder to complete we think that these requirements may be completed by the
  Notification feature in frappe. Me and pranvir just check it and we
  see that we can apply the condition in the "Condition" field. But this does not work for us.
-  Then we find one more solution that, there is a feature in client script called frappe.msgprint(). This function can be used with some conditions, so we can apply our conditions here.
-  Firstly we follow this link https://discuss.erpnext.com/t/client-script-to-fetch-value-from-another-doctype/1095/3 tutorial, to get alert message in sales invoice. In this tutorial we use one script and we test it on **gne12.gndec.ac.in**.

# Daily-Work (15-11-22)
Before start work things that i learn are :
## 1) Connection in doctype:
Inorder to make connection we have to link two
Stock work 12:00 -

# Daily-Work (17-11-22)

- In the morning, I learn from my team member that how we can apply condition  in the doctype ,like we have to do one task that get the alert message when total bill(sales invoice) is greater then the estimate cost. 
- I do discussion with team about student data or informtion because we have to add the hosteler(student) in the CMC project.So just create 5,6 student then enroll them in their respective program(CSE,MBA etc) and course(subject).This work com eunder the Education Domain in the erp.
- In the afternoon there was a meeting with teachers(Mentors) about our task and guidlines.In the meting we put our points and did the discussion about the project.
- Now my task was to upload the user(employee)on erp.So this work is done through Data import list ,where i  download the template according to requirment and put the provided data in the downloaded template and save it with .csv extenstion.There was  many  problem faced by me while uploading the user which are:
1) In the first time it showing the error that **The following values do not exist for Department: Computer Science Engineering – GNDEC**
2) Error regarding the User id of user(employee) which was their e-mail.

# Daily-Work (18-11-22)

- Today at morning 8:30 uploading the left user on erp.gndec.ac.in
- 9:00 Disscuss the CMC project with team.
- 10:25 Disscuss the Nankana Project with Satinder sir and had a meeting with Nankana School officals at 11:15.
- 11:15-12:26 In the meeeting we show our work to them and get their views on it and their requirements.
- 12:38 Discuss a problem related to the guru.gndec.ac.in with Amarpreet Mam(MBA Block).
  
  Working on rest of work.
  
# Daily-Work (19-11-22)
  
 - Today we went to the Nankana School and had the meeting with teachers .In the meeting they show us their feebank software and school fee structure.
 - In the evening their was seminer of other GD members .

# Daily-Work (21-11-22)

- Start working on Nankana Public school project and trying to meet their requirements in student applicant form.
- 10:32 -  The first thing they want in sibling  details  table is that
they only want to select the student ID and other details of selected
student come accordingly.This  work is done , now we only have to select the
student id and corresponding to this  First ,last name ,gender and
date of birth is come accordingly.
- Set the stock problem in erp.gndec.ac.in ,like disable the unwanted item .
- Trying to solve the error in quotion , like it was give the error of multicurrency _ invoice while creating the sales invoice.

# Daily-Work (22-11-22)

- Working on Education domain like Student Admission ,Fees.
- Did some work on guru.gndec.ac.in, solved the problems faced by teacher regarding participents in the courses.
  
# Daily-Work (23-11-22)

- Today i make connection of fee on student applicant form.
- Work on Fees Structure and make some program and fee category.

# Daily-Work (24-11-22)

- Make some LDAP user then upload and enroll them in their respective courses.
- Make duplicate of student applicant form to do same changes without changing the core of form.
- Make refrence workflow to understand the process and discuss it with Komal.

# Daily-Work (25-11-22)

- Today , I work on Nanak School project :

 1. Create the doctype Applicant Form ,add the connection of Applicant
fee in the doctype.

 2. Did some work on a CMC project like Company address and learned one
thing that we can we a customer an internal customer under
representing company from @ Rai sir.

 3. Create one more doctype Registration Form and also add the
connection  form where Applicants who submit the applicant fee can
submit his/her registration fee (5000).
Things now i am going to do is that in the registration fee form ,fee component fetch automatically while selecting the fee structure.

# Daily-Work (26-11-22)

- Today ,I am going to set the  view of the dashboard for the accountantmam(Nankana School Teacher). After this i will work on fee structure and fee         concession according to the school.

# Daily-Work (28-11-22)

- This morning all SDC members had a meeting  (google meet) with Satinder Sir regarding work progress . So in the meeting we discussed our problem  and    work status with sir.In our task (School project), sir told us to make workflow for applicant and registration forms instead of making different doctype
for each stage. Set permissions under it until the applicant did not deposit 500/- could not be able to open the registration form. Similarly if    registration has been completed only then he/she is able to see the enrollments.
So, now we(Jasjit, Komalpreet) are working on it .

# Daily-Work (29-11-22)

- Today we had a discussion with @ Satinderpal Sir and sir told us that we have to do all the steps (applicant and registration fee )  in one
doctype.For this we have to make three connections (Applicant fee , Advance Fee or Registration fee , Admission fee) in one doctype so it will be easy for us to do all the steps accordingly.
- I made one doctype named Student Form in gne12 and added the three connections of fees which are shown after saving the form. These fees are Applicant Fee , Advanced Fee and Fee.
# Daily-Work (30-11-22)

- Today my task is to add an Action button of Approved , Reject and
Enroll button on student applicant doctype so that after submitting
the fees and applicant form we enroll the applicant in a program or
course.

# Daily-Work (1-12-22)

-  Last we discuss the Student Applicant process with @ Satinderpal Sir and sir said us to make the connection of fees on one doctype so accordingly to sir we create one doctype named Waheguru on gne2.gndec.ac.in under Education Domain . In this doctype we (me, Komalpreet) make the connection of Applicant fee, Advanced Fee.After saving the form these connections are visible  and then we submit the form.
Then the task was to add an action button on this, this action button was about Approved or reject the form and after applying the condition of approved or reject we update the form the enroll option to enroll the applicant in the Program.

- Now the problem we faced was that when we enroll the applicant by clicking on Enroll button on Waheguru doctype it shows that:
"Student Applicant NSPS-SESSION-2023-2024-00003 not found" So, we are going to resolve the conflict.
- I think that it is because there is no relation between Waheguru and Program Enrollment doctypes , so now I am going to see it and report here regularly if it work.

 # Daily-Work (2-12-22)
 
 - Today we crete the user for NSPS school. These user are the Teachers ,so give them Instructor role at last. The main motive was  to show the courses to the instructor. For this we have to create the program ,courses. 

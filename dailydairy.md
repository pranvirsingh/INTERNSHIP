# 👉 Day 1 (12/07/22)
Download Ubuntu 22.04v linux operating system from Ubuntu official website. Make bootable drive of Ubuntu desktop using a tool [VENTOY](https://www.ventoy.net) and then Install in my laptop. Install some needy applications for linux like vscode, vim, etc. Also Learn how to use vim editor(little bit).

# 👉 Day 2 (13/07/22)
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

# 👉 Day 3 (14/07/22)
- Read about the frappe framework from [link](https://www.frappeframework.com) , its functionalities and advantages along with its installation. Also read about Jinja2 framework for templates.

---

# 👉 Day 4 (15/07/22)
- Install frappe framework using this [link](https://github.com/D-codE-Hub/Guide-to-Install-Frappe-ERPNext-in-Ubuntu-22.04-LTS) and face some problems and errors. I got an error in ```sudo mysql_secure_installation``` command and resolve this by searching on google.

---

# 👉 Day 5 (18/07/22)
- Make an app **library_management** using command ```bench new-app <app-name>``` using this [tutorial](https://frappeframework.com/docs/v13/user/en/tutorial/create-an-app)
- Then create a site **library5.test** using command ```bench new-site <site-name>``` following this [link](https://frappeframework.com/docs/v13/user/en/tutorial/create-a-site)
- Then install app on siteby using command ```bench --site library5.test install-app library_management```
- To confirm if the app was installed, run the command ```bench --site library.test list-apps```

---

# 👉 Day 6 (19/07/22)
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

# 👉 Day 7 (20/07/22)
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

# 👉 Day 8 (21/07/22)
- Recreate the **Library Management System** website and study deeply the documentation of frappe framework.

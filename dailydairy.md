# :point_right: Day 1
## Installing LAMP in Arch Linux

### Steps for the installation of LAMP are :-

1. Installing Apache-web-server
    * Installing the Apache-web-server by using this command. ```sudo pacman -S apache``` in the terminal.
2. Install PHP dynamic server-side scripting language and its Apache module. 
    * ```sudo pacman -S php php-apache```
3. On the last step install MySQL database, choose 1 (MariaDB) community database fork then start and check daemon status.
    * ```sudo pacman -S mysql```
4. Now **LAMP** is installed in my system.

### Steps to secure MySql database

5. The next step is to secure MySQL database by setting a password for root account, remove anonymous users accounts, remove test database and disallow remote login for user root.
    * ```sudo mysql_secure_installation```
6. Verify MySQL database connectivity by running the following command then leave database shell with quit or exit statement.
    * ```mysql -u root -p```

 # README

 > **NAME**

Configure MySQL Workbench

 > **DESCRIPTION**


Before running the commands shown on this page, you should load the Bitnami stack environment by executing the installdir/use_APPNAME script (Linux and MacOS) or by clicking the shortcut in the Start Menu under “Start -> Bitnami APPNAME Stack -> Application console” (Windows). On OS X VMs, the installation directory is /opt/bitnami and OS X VM users can click the “Open Terminal” button to run commands. Learn more about the Bitnami stack environment and about OS X VMs.

NOTE: We are in the process of modifying the configuration for many Bitnami stacks. On account of these changes, the file paths and commands stated in this guide may change depending on whether your Bitnami stack uses MySQL or MariaDB.

Linux and macOS native installer users can identify which database server is used in the stack by running the command below:

Replace the installdir placeholder with the full installation directory for your Bitnami stack.
test -d installdir/mariadb && echo "MariaDB" || echo "MySQL"
Windows native installer users can identify which database server is used in the stack by checking for the presence of the installdir/mariadb directory. If present, the installer uses MariaDB and if not, it uses MySQL.

Depending on which database server (MySQL or MariaDB) is used by the installation, use the appropriate guides in our documentation for database-related operations.

NOTE: This section assumes that you have downloaded and installed MySQL Workbench.

To connect to your remote MySQL database server using MySQL Workbench, you have to allow remote connections to the server.

[Reference](https://docs.bitnami.com/installer/apps/civicrm/configuration/configure-workbench/)


  > **VISUAL**

![MySQL Workbench](https://docs.bitnami.com/images/img/components/mysql/mysql-mwb-1.png)

![Setup New Connection](https://docs.bitnami.com/images/img/components/mysql/mysql-mwb-2.png)

![Setup New Connection](https://docs.bitnami.com/images/img/components/mysql/mysql-mwb-3.png)


![MySQL Workbench](https://docs.bitnami.com/images/img/components/mysql/mysql-mwb-4.png)


  > **Once your MySQL server is configured to accept remote connections, you can connect to it using MySQL Workbench. Follow these steps:**

{

    Step 1: Launch MySQL Workbench.
  

}

{

    Step 2:  Click the “+” symbol in the “MySQL Connections” tab to add a new connection.

    

}

{

    Step 3: Configure the connection as follows:
    
    * Enter a name for the connection in the “Connection Name” field.

    * Select “Standard (TCP/IP)” as the “Connection Type”.

    * Enter your server’s IP address in the “Hostname” field.

    * Specify the “Port” as “3306”.

    * Specify the “Username” as “root”.

}

{

    For Ubuntu servers:
    sudo apt install phpMyAdmin

    For CentOS
    First and EPEL repository and then run yum install phpmyadmin.

}

{

    Step 4: Click “Test Connection” to test the connection.




{
    
    Step 5: If the connection is successful, click “OK” to save the connection.

}



    Step 6: Double-click the new connection to launch the MySQL Workbench SQL Editor. You may be prompted for a password. Use the same password you used when previously configuring the server to accept remote connections. Once connected, the SQL editor window will open and you can interact with the server using SQL commands.

   

}

> **AUTHOR**

Author Name: Julliose Benedict S. Urbano

![DATABASE](https://scontent.fceb2-2.fna.fbcdn.net/v/t1.6435-9/77271638_1783660931769583_2812217188100866048_n.jpg?_nc_cat=104&ccb=1-5&_nc_sid=174925&_nc_eui2=AeF9rOJwUC66yZQirUyeoDHnjQbVO6PrDHWNBtU7o-sMdTGNkYMp7keFn-ths0BIqfvJQ83RLh6Cfcl_v2twVcjh&_nc_ohc=IV_wJ1_Ms98AX95qk4o&tn=fmytJamxHN2p3XwR&_nc_ht=scontent.fceb2-2.fna&oh=73be9e0826d548016e890be9067e4b6e&oe=61C3F4E4)

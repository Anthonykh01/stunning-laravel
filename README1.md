check point 1:
sudo apt install apache2 mysql-server .....
note::php-mcrypt gave an error 
tried install php7.1-mcrypt didn't work 
a2enmod rewrite
sudo service apache2 restart

check point 2:
cd /var/www/html
pwd
sudo git clone + diretory

check point 3: 
the given command does not work 

composer install 

check point4
pwd 
cp .env.example .env 
nano .env
php artisan ...

check point 5
apache2 -v 
sudo find / -name/apache2
cd/etc/apache2
ls
nano aache2.conf didn't work 
sudo vim apache2.conf 
cd sites.enabled
sudo vim 000....
sudo service apache2 restart

chech point 6:
cd/var/www/html/stunning-laravel
sudo chgrp -R www-data storage bootstrap/cache:
Laravel storage path permissions. This script makes storage path writable for both users, the admin and PHP Webserver user
The command "sudo chgrp -R www-data storage bootstrap/cache" changes the group ownership of two directories in a Laravel application: "storage" and "bootstrap/cache".

Here's a breakdown of what each part of the command means:

"sudo" is a command used in Unix-based systems to execute a command with elevated permissions (i.e., as a superuser). In other words, it allows the user to perform administrative tasks that require higher privileges.

"chgrp" stands for "change group" and is a command used in Unix-based systems to change the group ownership of files and directories.

"-R" stands for "recursive" and means that the command should be applied to the directories and all of their subdirectories and files.

"www-data" is the name of a Unix group commonly used for web servers, such as Apache or Nginx. This command changes the group ownership of the directories to the "www-data" group.

"storage bootstrap/cache" specifies the directories that the command should be applied to.

In summary, the command changes the group ownership of the "storage" and "bootstrap/cache" directories and all of their contents to the "www-data" group. This is often necessary in a Laravel application to ensure that the web server has the necessary permissions to read and write to these directories, which are used for caching and storing files. By changing the group ownership to "www-data", the web server will be able to access these directories and perform the necessary tasks.
---------------------------------------------------------------------------------------------------------------------------------------------------------------------
---------------------------------------------------------------------------------------------------------------------------------------------------------------------
The command "sudo chmod -R ug+rwx storage bootstrap/cache" changes the file permissions for two directories in a Laravel application: "storage" and "bootstrap/cache".

Here's a breakdown of what each part of the command means:

"sudo" is a command used in Unix-based systems to execute a command with elevated permissions (i.e., as a superuser). In other words, it allows the user to perform administrative tasks that require higher privileges.

"chmod" stands for "change mode" and is a command used in Unix-based systems to change the access permissions of files and directories.

"-R" stands for "recursive" and means that the command should be applied to the directories and all of their subdirectories and files.

"ug+rwx" specifies the new permissions to apply to the files and directories. "u" stands for "user", "g" stands for "group", and "+rwx" means to add read, write, and execute permissions.

"storage bootstrap/cache" specifies the directories that the command should be applied to.

In summary, the command changes the file permissions for the "storage" and "bootstrap/cache" directories and all of their contents, giving the user and group read, write, and execute permissions. This is often necessary in a Laravel application to ensure that the application has the necessary permissions to read and write to these directories, which are used for caching and storing files.


















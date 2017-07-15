## Run PhpMyAdmin:
- download and install xampp
- open Applications/XAMPP/manager-osx
- run mysql & apache 
	- if can't run apache:
	 - 1) sudo apachectl stop 
	 - 2) change ports from 80 to 81
 	- if can't run mysql:
	 - 1) sudo launchctl load -F /Library/LaunchDaemons/com.oracle.oss.mysql.mysqld.plist
	 - 1.1) or:
	 - 2) sudo /usr/local/mysql/support-files/mysql.server stop
- open localhost:80/dashboard - if you have apache on another port put it here


> On Nastya.Air port was changed to 81!


> THEN FOLLOW TO PICTURES to setup virtual port and run applications from specific FOLDER, with specific URL,
> like hazantip.local:81/

## to open httpd.conf:
	go to xampp - manage servers tab - apache select - configure - open conf file

## to get hosts:
	sudo vi /etc/hosts

## PhpMyAdmin permission denied(13):
	Applications/XAMPP/xamppfiles/temp - CMD + I - add rights to user which you typed in httpd.conf

# Images

***
![apache-port](/apache-port.png)
***
![httpd.conf.vhost-fix](/httpd-conf-vhost-fix.png)
***
![httpd.conf-vhost-enable](/httpd-conf-vhost-enable.png)
***
![etc/hosts](/etc-hosts.png)
***
![httpd.conf-fix2](/httpd-conf-fix2.png)
***
![phpmyadmin-temp-rights](/phpmyadmin_temp_rights.png)

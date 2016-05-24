LinuxServerConfiguration

Public IP Address : 52.40.80.9

Port : 2200

Passphrase: appuser

URL : 
- http://ec2-52-40-80-9.us-west-2.compute.amazonaws.com/
- http://52.40.80.9

Installed Packages

1) finger:	Displays an easy to read information about a user   
2) apache2:	HTTP Server   
3) libapache2-mod-wsgi:	hosts Python applications on Apache2 server   
4) ntp: Synchronizes time over a network   
5) postgresql: Postgresql Database server   
6) python-setuptools: An easy-install package to facilitate installing Python packages   
7) sqlalchemy: ORM and SQL tools for Python   
8) flask: Microframework for web applications   
9) python-psycopg2:	PostgreSQL adapter for Python   
10) oauth2: Authorization framework for third-party login   
11) google-api-python-client: Google API for OAuth login   
12) fail2ban: Protection against suspicious site activity by IP banning   

Configuration Summary

1) Created a new user named grader   
2) Updated and Upgraded currently installed packages   
3) Changed the ssh port from 22 to 2200   
4) Gave the grader perminsiion to sudo   
5) Configured the Firewall (UFW) to only allow incoming connections for SSH (port 2200), HTTP (port 80), and NTP (port 123)   
6) Configured the local timezone to UTC   
7) Installed and configure Apache to serve a Python mod_wsgi application.   
8) Set up Environment for delopying Flask Application.   
9) Installed and configured PostgreSQL with default settings to not allow remote connection.  
10) Created a new user catalog, added user to PostgreSQL databse with limited permissions to catalog application database.   
11) Installed and Configured Fail2ban intrusion protection that bans suspicious IPs.   

Resources
- https://www.digitalocean.com
- https://github.com/elnobun/Linux-Server-Configuration
- https://github.com/stueken/FSND-P5_Linux-Server-Configuration
- https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps
- http://stackoverflow.com/questions/10572498/importerror-no-module-named-sqlalchemy
- http://stackoverflow.com/questions/12906351/importerror-no-module-named-psycopg2

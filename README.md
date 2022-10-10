# Retailshop
Retail Shop Software - Java Swing - MySQL 

# Youtube Video Link
https://www.youtube.com/watch?v=LvAZADOUtzQ&t=1473s

# Installation Procedure

#### Create Folder

-> Create 'MSquaresys_Software' folder
-> Keep all the downloaded files into MSquaresys_Software
-> Check OS is 32-bit and 64-bit
	Install 'jdk-8u201-windows-x64.exe' if OS is 64-bit
	Install 'jdk-8u201-windows-x84.exe' if OS is 32-bit


#### Java Installation

NOTE: Before Java installation, check java is already installed in OS or not ( if java version is above 1.8, do not install)

1. Install jdk-8u201-windows-x64.exe   (Run as administrator)

2. After successful installation, open command prompt  

Run -> command 
	
C:\Users\Admin>java -version      (## verify the java version is proper)

java version "1.8.0_201"
Java(TM) SE Runtime Environment (build 1.8.0_201-b09)
Java HotSpot(TM) 64-Bit Server VM (build 25.201-b09, mixed mode)

#### MySQL Installation

3. Install mysql-installer-community-5.7.17.0.msi   

-> Select Server option

During installation, mysql installer ask root password that is "mysql" only
 
   Create root password : mysql


#### Sqlyog Installation

4. SQLyog-12.1.5-0.x86Community   (Run as administrator)

5. Open sqlyog   (After successful installation)

	Type in search prompt : sqlyog
	
	Create New (by pressing the 'new' button)
	
	Saved Connection : bill_db

	Mysql Host Address: localhost
	
	Username	: root
	
	Password	: mysql
	
	Port		: 3306
	
					<<Test Connection>>    
					
(If test connection is success, it shows "connection successful")

-> Import the data   (ms_import.sql)
	(Right click the browser tree root@localhost :: left side)
	(Select the menu option as 'Execute SQL script')


#### Run the java jar

6. execute TileApps.jar  

7. Testing in command prompt

	java -jar TileApps.jar  
	
### Create shortcut

8. Create shortcut for TileApps.jar and rename the schortcut into 'MSquaresys Software'

9. Change shortcut Icon (desktop.ico)

10. Copy the shortcut and keep it in desktop  


### Final

double click the desktop shortcut('MSquaresys Software') and execute the billing software


### Change the property files  (myapp.properties)  :: 

We can edit this properties in software itself  (Login into software -> More features -> User Settings)

Update the customer(who purchased the MSquaresys software) details

Open the file myapp.properties in notepad

#### hints (myapp.properties file)

app.db   	- is mysql database name   (tilesapp)
app.gst  	- is gst percentage  (10%)
app.roll 	- is roll print enabled (yes)  - keep 'no' for disable the roll print
app.a4		- is A4 Sheet print enabled (yes) - keep 'no' for disable the A4 print
app.foot    - is empty text by default (Tag name text will appear in bill receipt)
app.comm    - is comment text in the bill receipt (Thanks for shopping with us)
app.user    - is mysql database user   (root)
app.pass    - is default app user password (msquare) - when new user is added, then that user password is msquare
app.land    - is landmark name - Near by location to customer (who purchased the MSquareSys software)
app.gstn    - is customer GST number
app.cont    - is customer contact number (add more contact no by using comma separator)
app.mail    - is customer mail id
id.prefix 	- is customer shop id prefix (default 'MS' - abbreviation is MsquareSys)  :: MS001, MS002 - Software login ID
app.title   - is MSquareSys software name 
app.dbpass  - is mysql database password
app.port	- is mysql port number
app.header  - is software title (MSquareSys)
app.cond	- is condition text in the bill receipt (Damaged items should not be returned) 
app.loc		- is customer location/place name (Surandai, Serndamaram, etc)
app.host	- is mysql server hostname/IP

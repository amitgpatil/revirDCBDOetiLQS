# revirDCBDOetiLQS
tniM xuniL rof revirDCBDOetiLQS 

RefSource is used to create trunk project. This is tested on Linux Mint 18.1 serena. 
---------------------------------------------------------------------------------------
-----------------------------Getting Started-------------------------------------------
---------------------------------------------------------------------------------------
About project -
This project can be used to develope SQLite ODBC Driver for windows 32 bit and 64 bit on Linux Mint 18.1 64 bit.
Credit goes to http://www.ch-werner.de/sqliteodbc/ 


Source code used for project:
1. SQLite ODBC Driver : 
	http://www.ch-werner.de/sqliteodbc/sqliteodbc-0.9995.tar.gz
	
2. SQLite database engine source code (older versions):
	https://www.sqlite.org/chronology.html
	
3.SQLite extension functions:
	http://www.sqlite.org/contrib/download/extension-functions.c?get=25
	

Folder structure of the project:	
Above source code is placed inside RefSource folder in extracted format and in renamed folders according to the script.
Trunk contains working files which is used to generate executables. This contains SQLite ODBC Driver code primarily.
Other folders will be copied and used according to the script.

Building the project:
1. Preparing machine - Installing Linux Mint 18.1 on windows:
   a. Keep one drive with 100GB free space
   b. Download iso from https://www.linuxmint.com/download.php
   c. Create bootable on USB .Google for steps
   d. Install. 
   
2. Installing pre-requisites:
   a. Install GCC: 
       amit@amit-mint ~ $ sudo apt-get install g++
	   
   b. Install mingw-w64 for Linux Mint:
      https://community.linuxmint.com/software/view/mingw-w64

   c. Install nsis installer making utility:
      https://community.linuxmint.com/software/view/nsis
	  
3. Running script to make dlls and exes:
       amit@amit-mint ~ <complte path of mingw64-cross-build.sh> file.
	  

Customizing the project:
1. Change version using file VERSION
2. Change properties by changing .RC files  AND .def and sqlite*odbc.h and .c files (Optional - need only if total change in nomenclature required !)	  



# odbcunshackler2

Expose your Windows-only ODBC databases over an HTTP interface

ODBC Unshackler 2 uses [PyODBC](https://github.com/mkleehammer/pyodbc) to 
interact with your ODBC databases on Windows. Flask is run as Windows service 
or via command line to provide an HTTP interface. You specify a SQL query in 
the URL of your HTTP request, and the results of the queries are returned via 
JSON in the response. No authorization or authentication mechanism is provided. 

# Legacy Windows

It is likely that this program will be used to expose ODBC databases on legacy 
versions of Windows such as Windows XP. In light of this, the program targets 
[Python 3.4](https://www.python.org/download/releases/3.4.0/), which is the 
last version of Python available for Windows XP.

There has been no attempt to backport this program to Windows 2000, Windows ME, 
or Windows 98. Sorry, you're on your own with those.

CS3130 Assignment 4
Janelle Montgomery

A TCP-based client and server that accesses a database. You will be able to modify the database using : search,add,remove,and display. To do this TCP based protcol will be used.

This program is meant for a user to understand how TCP works over the server. It has a separate recv_all function in order to handle the data being sent to the client from the server. This is what makes sure the TCP connection is reliable and that all data is being sent. It does this by checking if the terminator is in the data. In my case I chose to use a "." to show that all data has been recieved.

The protocol that I have set us is:

Client:

+800: Add a user to the database
+810: Search for a user in the database
+820: Remove a user from the database
+830: Display all users in the database
+840: Quit the program <Client and Server>

Server:

+310: User has successfully been added to the database
-300: The user has not been added and already exists
+410: User was successfully found in the database
-400: Not a valid employee in the database
+510: Remove from the database was successful
-500: Not a valid employee in the database
+610: Display the entire content of the database

In order to run this program you may type: python3 tcpmsg.py client/server in the Terminal window.

Github URL: https://github.com/JanellePearl/cs3130_LabAssignment4


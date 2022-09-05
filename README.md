# Client-Server-Trading-System

This application contains following files
--------------------------------------------------------
--> server.c - C code file for server
--> server.h - header file for server 
--> client.c - C code file for client
--> credentials.txt - contains login credentials (trader id, user name, password)
--> makefile - for compiling client and server code.


Compiling files
--------------------------------------------------------
For Server ::::::::
make server

For Client ::::::::
make client

Executing 
--------------------------------------------------------
For Server ::::::::
./server <SERVER PORT NUMBER>

For Client ::::::::
./client <Server IP Address> <SERVER PORT NUMBER>

---->use a port number greater than or equal to 1024

********************************************************

Client Queries thats servered by the server
     -> Credential verification: Typed username and passwords are first verified using the credential.txt file
     -> After verification Trader ID is also asked 
     (First column in credential.txt is the Trader ID, second column is user name and third column is password)
     -> Asked responses are seperated by white spaces 

Request Types -------------------------------------

     -> Login request
          <Log-IN ID> <PASSWORD> L $

     -> Buy request
          <Log-IN ID> <PASSWORD> B <item-code> <qty> <unit-price> $

     -> Sell request
          <Log-IN ID> <PASSWORD> S <item-code> <qty> <unit-price> $

     -> View Trades
          <Log-IN ID> <PASSWORD> VT $

     -> View orders
           <Log-IN ID> <PASSWORD> VO $



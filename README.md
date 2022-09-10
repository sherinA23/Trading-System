# Client-Server-Trading-System

A Client-Server based Trading System application, developed using socket programming

Compiling files
--------------------------------------------------------
**Server:**
```$ make server```
>Creates an executable with the name  "server"
    
**Client:**
```$ make client```
>Creates an executable with the name "client"

Executing 
--------------------------------------------------------
**Running Server:**
```$ ./server \<SERVER PORT NUMBER>```
>Use port numner >= 1024

**Running Client:**
```$ ./client \<Server IP Address> \<SERVER PORT NUMBER>```

********************************************************
- Credential verification: Typed username and passwords are first verified using the credential.txt file
- After verification Trader ID is also asked. (First column in credential.txt is the Trader ID, second column is user name and third column is password)
- Asked responses are seperated by white spaces 

Supported Request Types -------------------------------------
```
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
```


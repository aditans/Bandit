# LVL 14 --> 15
## APPROACH
1. using ls we couldnt find any files. 
   
2. So for sending the password to bandit we might need a nc (net cat) to establish the connection.






## CONCEPTS
 
### nc :netcat:
it can be used for sending about anything the sun involving Tcp or UDP. It can open tcp under connections, send upd packets, listen on arbitrary TCP/ UDP ports. 

              syntax : nc <host> <port no>

flags:

     1. - u : uses Udp insted of TCP. 
     2. - s : source's IP add.
     3. - 4 :forces nc to use IPv4 addresses only  
     4. - 6 :forces nc to use ipV6 addresses only
     5. - l listening for connections.


 ## STEPS

1. nc localhost -30000
2. enter bandit14 password 

    
 ## LINKS:

https://www.tutorialspoint.com/unix_commands/nc.htm

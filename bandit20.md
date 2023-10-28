# LVL 20 --> 21
## APPROACH
1. We can find suconnect file in the bandit20 dir.
2. Now upon its execution it makes a connection to the localhost on the port we specify.

3. It will transmitt password for next lvl only if the password for bandit20 is been encieved from the listener's port.

4. we might have to create a listening server and connecting user client.

5. We can do that by nc-l.

6. The connection has to be made from local host to local host.


## CONCEPTS
 
### nc : netcat:
used for tcp/udp or for listening.

flags:
  
     -l : listening 
     -p : port no.
     -v : produce more verbose output

   

 ## STEPS

1. on one command line window connect to bandit20 and write:


                          nc -lvp 3000

2. on another command line window connect to bandit20 and write:

                        ./suconnect 3000

3.then type the current lvl password in the listener window to get the password for next lvl. 

      
 ## LINKS:

https://www.youtube.com/watch?v=hlAQQPfSew0&list=PLG44s1Oo_jbTzrJ4kI24LwAyjFtTSDNlq&index=22&pp=iAQB
# LVL 13 --> 14
## APPROACH
1. We need to establish connection with bandet senver with our private kay. 
2. To do so we might need to use different command than ssh.





## CONCEPTS
 
### ssh:secure shell: 
used to connect to a remote Server.

flags:

    a. -1: Use protocol 1 
    b. -2: use protocol version 2 only. 
    c. -4: use IPv4 address 
    d. -6: use IPv6 add. 
    e. -i: identity file private key is taken from.


 ## STEPS

1. locate sshkey.private 
2. ssh bandit14@bandit.Labs.overthewire.org -p 2220 -i sshkey.private 

    
 ## LINKS:

https://www.ssh.com/academy/ssh/command

# LVL 16 --> 17
## APPROACH
1.  There are no files present.

2.  They are asking asking us to scan b/w 31000 to 32000 to  search for listening ports. 
   
3.  After that searching among them for SSL speaking servers. 
4.  We might have to use nmap as it can also portscan.



## CONCEPTS
 
### nmap
Nmap is Linux command-line tool for network exploration and security auditing. This tool is generally used by hackers and cybersecurity enthusiasts and even by network and system administrators

              syntax : nmap -flags (domain.name)

flags:

     1. -r : scan consecutively
     2. s_server : implements a generic ssl/tls server
     3. -A : enable os detection,tracework
     4. -sS: tcp scan
     5. -p (port range): scans b/w the range


 ## STEPS

1. nmap -p 31000-32000 localhost 

2. nmap -A - p 31000 - 32000

3. openssl s_cient -connect localhost: 31790

4. chmod 700 (filename)

5. ssh bandit17@bandit.labs.overthewire.org -p 2220 (filename)
   

    
 ## LINKS:

https://www.geeksforgeeks.org/nmap-command-in-linux-with-examples/
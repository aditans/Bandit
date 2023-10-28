# LVL 15 --> 16
## APPROACH
1. using ls we couldnt find any files. 
   
2. we have to use tcp again

3. This time we have to use openssl command as encryption is given in the question.



## CONCEPTS
 
### openssl
OpenSSL is an open-source command line tool that is commonly used to generate private keys, create CSRs, install your SSL/TLS certificate, and identify certificate information.

              syntax : openssl (commands) -flags (parameters)

flags:

     1. s_client : implements a generic ssl/tls client
     2. s_server : implements a generic ssl/tls server
     3. -connect (host:port) 
     4. - h : host add.
     5. - p : port no.


 ## STEPS

1. openssl s_client -connect localhost:30001
   

    
 ## LINKS:

https://www.digicert.com/kb/ssl-support/openssl-quick-reference-guide.htm
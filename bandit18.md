# LVL 18 --> 19
## APPROACH
1. Upon entering the password, the server keeps loging out.

2. This is because of a hidden file .bashrc in our home directory.

3. someone modified .bashrc file.



## CONCEPTS
 
### ssh (command)
 if a command is specified,it will be executed on the remote host instead of a login shell. 

### bash
its a shell for kernel distribution linux. It interprets the commands and gives them to the os to process. Whenever a shell is launched it loads a startup script thats defined in .bashrc or .bash_profile
              
              
    

 ## STEPS

1. ssh bandit18@bandit.labs.overthewire.org -p 2220 cat readme

      
 ## LINKS:

https://www.youtube.com/watch?v=xhZ9lp2uAL8&list=PLG44s1Oo_jbTzrJ4kI24LwAyjFtTSDNlq&index=20&pp=iAQB

# LVL 19 --> 20
## APPROACH
1. search for file in band20 
2. found bandit20-do file, but we can read it because of its permissions. 
3. but it has 's' in owner's id (setuid).

4. it always sets the user to owner, while executing that command.

5. But after using ls-al we see that this file Can only be executed by bandit 19 but we are bandit 19 right?

6. So, that means upon execution it sets our user from bandit 19(user) to bandet 20 (owner).

7. We can med recheck this by typing  "whoami" & "./bandi20-do whoami "



## CONCEPTS
 
### ./
used for execution of a file

   

 ## STEPS

1. ./bandit20-do cat /etc/bandit-pass/bandit20
      
 ## LINKS:

https://www.youtube.com/watch?v=Z-LXtVHowqo&list=PLG44s1Oo_jbTzrJ4kI24LwAyjFtTSDNlq&index=21&pp=iAQB
# LVL 17 --> 18
## APPROACH
1.  Using ls we found two files.

2.  it says to check for the only different line in both files. 
   
3.  we can use diff command for this.



## CONCEPTS
 
### diff
 This command is used to display the differences in the files by comparing the files line by line. Unlike its fellow members, cmp and comm, it tells us which lines in one file have is to be changed to make the two files identical. 

              syntax : diff -flags (file1) (file2)
              
              
1. Lines preceded by a < are lines from the first file.
2. Lines preceded by > are lines from the second file.
   

special symbols:

     a : add
     c : change
     d : delete

flags:

     1. -c : context : to see the modification date and time
     2. -i : to make it case sensitive.
    

 ## STEPS

1. diff passwords.old passwords.new (the line with > is our password)

      
 ## LINKS:

https://www.geeksforgeeks.org/diff-command-linux-examples/
# LVL 12 --> 13
## APPROACH
1. using ls to find data.txt
   
2. opening it to find, its a hexdump! 
   
3. making a new directory under tmp, to so that it would make it easier for us to work & decompress files.

1. Navigating to emp.

2. moving data.txt to tmp

## CONCEPTS
### mv: 
To move a file or directory to another location. To rename a file.

         syntax : mv (file1) (file2) (destinatn path) 


  flags: 

         a. -i: asks for confirmation 

         b. -n: doesn't overwrite. 
        
         c. -b: takes backup of an on an existing file that will be overwillen.

## xxd:
creates a hex dump of a given file or does the reverse.


         Syntax : xxd -flags (inpfile) (outfile).

flags:

         a. -b: bits: instead of hexdump it switches to binary digits.

         B.-E: changes character encoding from ASCII to EBCDIC.

         C. -r: revesse hex dump.

## gzip:
used to compress files or decompress..

                   syntax :gap flags (file)

flags:
         a. -f: forced compression of already file.gz exists gzip would doesn't works, but using thisit would compress forefully.Overwires date.

         b. -L: lisence

         c. -r (directory) :compreses every file in that directory.

## bzip2:

slower decompression time & higher. memory use. It usually achieves a higher compression ratio than grip. but is also slower & more CPU-intensi

                   Syntax: bzip2 -flags (file)

flags:

    1. -k: des compress but alre the og file 2.-d: decompression (hakes only. 622) s:t: chuck integrity

    2. -V: shows compression ratio
    
    3. -d: decompress

    

## tar: 
used to create archieve or extract archive files.

    syntax : tar -flags (archivefile) (locatn or diratory to be archived)

flags:
   

    -c:Creates an archive by bundling files and directories together.

   
     -x: Extracts files and directories from an existing archive.

     -f: Specifies the filename of the archive to be created or extracted.

     -z :Uses gzip compression when creating a tar file, resulting in a compressed archive with the ‘.tar.gz’ extension.

     -j: Uses bzip2 compression when creating a tar file, resulting in a compressed archive with the ‘.tar.bz2’ extension.



 ## STEPS

1. find data.txt

2.  mkdir /tmp/bigth

3.  xxd -r data.txt /tmp/bigth/datal.txt

4.  cd tmp/bigth 
   
5.  file datal.txt (it will show compressed by gzip)

6.  mv datal.txt data2.bin.gz

7.  gzip -d data2.bin.gz ( which would give us data2.bin)
    
8.  file data2.bin ( it'll show bzip2 compressed)

9.  mv data2.bin datu2.bin.bz2

10. bzip2 -d data2.bin.bz2 (ill give us data2.bin) 
    
11. file data2.bin (ill show gzip compressed data)

12. mv data2.bin data4.bin.gz

13. gzip -d data4.bin.gz (ill give us data4)

14. file data4.bin (ill show us archived by tar)
    
15. mv dada4.bin data4.bin.tar

16. tar -x -f data4.bin.tar
     
17. file data5.bin
    
18. mv data5.bin data5.bin.tar
    
19.  tar -xf data5.bin.tar (ill give us data6-bin)

20. file datab.bin      (ill show us bzip2 compressed.) 
    
21. mv data6.bin  data6.bin.bz2
    
22. bzip2 -d data6.bin.bz2 (ill give us data6.bin)
    
23. file data6.bin (ill show us archived by tar).

24. mv data6.bin data6.bin.tar

25. tar -xf data6.bin.tar (ill give us data 8.bin)

26. file data8.bin (ill show us grip compressed was data9)
    
27. mv data6.bin data9.bin.gz

28. gz -d data9.bin.gz (ill give us data 9.bin)

29. file data9 bin (`ill show us ASCII text! finally)

32. cat data9.bin  
    
 ## LINKS:

https://www.geeksforgeeks.org/tar-command-linux-examples/
https://www.geeksforgeeks.org/gzip-command-linux/
https://www.geeksforgeeks.org/bzip2-command-in-linux-with-examples/


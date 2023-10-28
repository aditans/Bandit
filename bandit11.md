# LVL 11 --> 12
## APPROACH
1. find data.txt

2. opens it and sees a POT13

3. Thinking of solving this encryption using tr.

## CONCEPTS
### tr: 
for translating, deleting, squeezing repeated characters & basic find and replace. It basically finds characters from set 1 & replaces them by their equivalent character in Set 2. The main disadvantage is tht it only takes i/p interms of file or Piping.

       a. -s: squeeze: removes repeated sequences.

       b. -d: deletes specified string.

       c. -cd: complement: To remove all the characters except the mentioned one.

       d.-t: turncate.

 ## STEPS

1. find data.txt

2. cat data.txt | tr "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ" "nopqrstuvwxyzabcdefghijklmNOPQRSTUVWXYZABCDEFGHIJKLM"

                    or if simplified: 

2. Cat data.txt | tr "a-zA-Z" "n-za-mN-ZA-M"

## LINKS:

[•devicetests.com/decode-rot13-text-command-line.](https://devicetests.com/decode-rot13-text-command-line)
  


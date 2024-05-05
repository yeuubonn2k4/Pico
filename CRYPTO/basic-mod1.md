## Description

We found this weird message being passed around on the servers, we think we have a working decryption scheme.
Download the message here.
Take each number mod 37 and map it to the following character set: 0-25 is the alphabet (uppercase), 26-35 are the decimal digits, and 36 is an underscore.
Wrap your decrypted message in the picoCTF flag format (i.e. picoCTF{decrypted_message})

128 322 353 235 336 73 198 332 202 285 57 87 262 221 218 405 335 101 256 227 112 140 

## Solution

- - Lan luot lay cac so chia du voi 37 thi duoc 17 26 20 13 3 36 13 36 17 26 20 13 3 36 33 35 2 27 34 5 1 29

- - Neu 0-25 thi la abc....

- - Neu 26-35 thi la 0123456789
 
  - 36 la _
 
    Flag

    `
    picoCTF{r0und_n_r0und_79c18fb3}

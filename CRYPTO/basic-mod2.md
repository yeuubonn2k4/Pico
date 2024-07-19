## Description

A new modular challenge!

Download the message here

https://artifacts.picoctf.net/c/178/message.txt

Take each number mod 41 and find the modular inverse for the result. Then map to the following character set: 1-26 are the alphabet, 27-36 are the decimal digits, and 37 is an underscore.

Wrap your decrypted message in the picoCTF flag format (i.e. picoCTF{decrypted_message})

## Solve

![image](https://github.com/user-attachments/assets/59111f43-fdc3-4784-a33c-1779d5720a9f)

Code

import string

alphabet = string.ascii_lowercase
alphabet += "0123456789_"
flag_enc = [432, 331, 192, 108, 180, 50, 231, 188, 105, 51, 364, 168, 344, 195, 297, 342, 292, 198, 448, 62, 236, 342,63 ]

flag = ""
for c in flag_enc: 
    pos = pow(c, -1, 41)
    flag += alphabet[pos-1]

print(flag)

}

Flag

`
picoCTF{1nv3r53ly_h4rd_c680bdc1}
`

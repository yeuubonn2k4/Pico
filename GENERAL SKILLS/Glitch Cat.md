## Description

Description
Our flag printing service has started glitching!
$ nc saturn.picoctf.net 58070

## Solution

![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/6c2d6aca-2e09-4170-adc2-67c69d3a0a70)

Trong python , chr la lenh bien so thanh ki tu

'picoCTF{gl17ch_m3_n07_' + chr(0x61) + chr(0x34) + chr(0x33) + chr(0x39) + chr(0x32) + chr(0x64) + chr(0x32) + chr(0x65) + '}'

Chay chung trong python ta duoc 

![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/c409661f-073a-43e3-9455-80ed1765944c)

Flag la

`
picoCTF{gl17ch_m3_n07_a4392d2e}
`

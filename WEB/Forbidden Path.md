## Description

Can you get the flag?
We know that the website files live in /usr/share/nginx/html/ and the flag is at /flag.txt but the website is filtering absolute file paths. Can you get past the filter to read the flag?
Additional details will be available after launching your challenge instance.

Here's the website.

http://saturn.picoctf.net:62613/

## Solution

![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/7b118997-9025-4997-a144-fd2cf2d8b859)

- Vi de bai cho ta dang o thu muc /usr/share/nginx/html/   

- Vi vay de tim duoc flag thi chung ta phai quay tro lai vi tri ban dau bang cach /../../../../ (thoat ra khoi 4 cai path kia)

- Sau do vao flag.txt

![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/f9839975-7d1b-4da6-8a63-c0945cb44f35)

![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/782a8157-2a9c-4289-a0bb-31ac7ec8ac8b)

Thu duoc Flag la 

`
picoCTF{7h3_p47h_70_5ucc355_e5fe3d4d}
`

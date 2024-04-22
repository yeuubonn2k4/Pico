There is some interesting information hidden around this site http://mercury.picoctf.net:27393/. Can you find it?

Ấn vào link sẽ tìm dc 2 flag là khi inspect

picoCTF{th4ts_4_l0

dựa theo gợi ý ở tệp .js

ta gõ

http://mercury.picoctf.net:27393/robots.txt

hiện key thứ 3 là  t_0f_pl4c

nó còn hiện thêm dòng I think this is an apache server... can you Access the next flag?

Ta nhận ra tệp mặc định ở Apache là .htaccess

hiện ra key là 3s_2_lO0k

nó thêm dòng chữ I love making websites on my Mac, I can Store a lot of information there.

Ta nhận thấy mặc định của Mac là .DS_Store

_d375c750}



Flags : picoCTF{th4ts_4_l0t_0f_pl4c3s_2_lO0k_d375c750}

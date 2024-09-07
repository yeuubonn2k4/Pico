## Description

Oracles can be your best friend, they will decrypt anything, except the flag's ciphertext. How will you break it? Connect with nc mercury.picoctf.net 2671.

## Solve

![image](https://github.com/user-attachments/assets/0a98d6b1-95d6-436d-88dd-268a3d2cf544)

![image](https://github.com/user-attachments/assets/e9458308-6c29-4266-a563-1df750ed23ce)

>>> n = 51257263015582188197648371474129549390905726426257438448153816359702362365658508334422660676137191608574589301862860723036048910648313371474365316649888203989162930646519011433136231329260451213231902920703710354241532734042339059649207865410951756937740333312020743615116676965217774179610963694893894058993

>>> e = 65537

>>> c = 4630900525813217788908324506108030714601444705261980401094718094759603138876572869225585464832937171107712654868912146981974620187638194979958086597403998901460677636640013168017847942623819676132193036153903064536382635689292213133256195449181769142311263486211152780709880862212814932262615707105931438936

>>> x = pow(2, e, n)

!![image](https://github.com/user-attachments/assets/18e472c1-f502-49ed-9795-32281a02da52)

580550060391700078946913236734911770139931497702556153513487440893406629034802718534645538074938502890769430290200460554490

- Sau khi chia 2 ta được

   290275030195850039473456618367455885069965748851278076756743720446703314517401359267322769037469251445384715145100230277245

`
  picoCTF{m4yb3_Th0se_m3s54g3s_4r3_difurrent_5814368}
`
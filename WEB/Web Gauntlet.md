### Note

If the flag is not displayed after completing this challenge, try clearing your cookies. 
Cookies set by other challenges may prevent the flag from displaying properly.

## Description

http://jupiter.challenges.picoctf.org:54319/

http://jupiter.challenges.picoctf.org:54319/filter.php

## Solution

- Khi ban dang nhap username la ` admin ` va mat khau bat ki no se hien nhu zayyy

  ![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/80256558-fc2f-4849-baee-35daf5ba95b2)

- Nhung hay chu y thu an dang sauuu

![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/b126bef3-3ecc-41e2-8959-f01437b6a056)

- Do la 1 truy van kieu SQL, biet ten admin roi thi usernam la admin'-- (su dung "--" thi sau no mat khau co la gi cung khong quan trong)

- Vi Comments trong SQL thường được sử dụng để:

Giải thích mã SQL: Bạn có thể sử dụng comments để giải thích ý nghĩa hoặc mục đích của một phần cụ thể trong mã SQL, giúp người đọc hiểu rõ hơn về mã.

Tạm thời loại bỏ một phần của mã: Bạn có thể tạm thời loại bỏ một phần của mã SQL bằng cách chuyển nó thành comment. Điều này hữu ích khi bạn muốn thử nghiệm hoặc debug một phần của mã mà không muốn xóa hoặc thay đổi nó.

- Nhap vao chung toi da qua duoc round 2

![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/1b06f66d-4398-4732-9835-2ce5247fc0df)

- Goi y round2 la

![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/c4198df5-b7e1-4b3a-8de1-baf8bfa819ad)

- Trong phần này, chúng ta không thể sử dụng - bình luận. Tuy nhiên, chúng tôi biết rằng đây là SQLite và có 2 loại nhận xét, — và /**/. Rõ ràng là chúng ta có thể chỉ cần sử dụng cái khác như chúng ta đã làm trước đây, chẳng hạn như:    

![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/56543049-9551-44a0-a19f-1bf5354a3521)

Bởi vì Mọi nội dung nằm giữa "/" và "*/" sẽ được coi là comment và sẽ không được thực thi như là một phần của câu lệnh SQL.

Comments nhiều dòng thường được sử dụng để:

Giải thích mã SQL phức tạp: Bạn có thể sử dụng comments nhiều dòng để giải thích mã SQL phức tạp hoặc những phần mã có logic phức tạp.

Tạo phần đầu ra dễ đọc hơn: Comments nhiều dòng giúp làm cho mã SQL trở nên dễ đọc hơn bằng cách phân chia nó thành các phần và giải thích mỗi phần.

- Chung ta da sang duoc round 3

![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/ffe123a1-ca5c-46cd-a328-bb3f8742be86)

- Goi y cua round nay la

![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/0876ca0c-b6f0-4d03-984d-968ad4947389)

- Co nghia la cu phap nao cung dung de binh luan nhu vay , do la ";"

- Dang nhap voi username la ` admin'; ` va da qua duoc round 4

![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/e3e0187f-633c-42aa-b3ce-98d5d6ccb538)

- Goi y cua round nay la

![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/0d161ef6-d08e-4014-af96-4c7eacf37b26)

- No nghia la khong cho su dung quyen "admin"

- Chung ta co the su dung ad'||'min'; phep || la phep noi trong SQL

- Ta da qua round 5

![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/3d79d840-a2ea-4b1d-8edd-07d5c9d20005)

- Goi y la

![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/d6595bbb-5dbf-4809-ac9b-c192ba6739d2)

Nghia la khong duoc su dung Union admin

- Toi lai go lai Round 4 nhu ad'||'min';

- Va toi den duoc Round 6/5

![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/9d1690a5-6645-4618-89e9-9ff70b388fb7)

- Va bay gio chi viec check filter.php

![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/e6e7ad23-64cc-4562-b396-266e8c10ea56)

- Ta co duoc Flag

`
picoCTF{y0u_m4d3_1t_a5f58d5564fce237fbcc978af033c11b}
`

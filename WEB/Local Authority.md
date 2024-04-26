Can you get the flag?
Go to this website and see what you can discover.
(http://saturn.picoctf.net:50262/)

![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/2c8639d3-8e22-4477-8311-07aef4bc4015)

Ctrl U ra 

![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/a96383c1-af81-470b-ac08-df68eb60df66)

doan no yeu cau zay 

![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/c875fda2-6192-4a51-a095-5b31fd4367d6)

co gang dang nhap sai bang cach nhap ki tu bat ki

![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/138e8022-b74a-49bb-9ecc-140fcef01c83)

Ctrl U

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <link rel="stylesheet" href="style.css">
    <title>Login Page</title>
  </head>
  <body>
    <script src="secure.js"></script>
    
    <p id='msg'></p>
    
    <form hidden action="admin.php" method="post" id="hiddenAdminForm">
      <input type="text" name="hash" required id="adminFormHash">
    </form>
    
    <script type="text/javascript">
      function filter(string) {
        filterPassed = true;
        for (let i =0; i < string.length; i++){
          cc = string.charCodeAt(i);
          
          if ( (cc >= 48 && cc <= 57) ||
               (cc >= 65 && cc <= 90) ||
               (cc >= 97 && cc <= 122) )
          {
            filterPassed = true;     
          }
          else
          {
            return false;
          }
        }
        
        return true;
      }
    
      window.username = "a";
      window.password = "b";
      
      usernameFilterPassed = filter(window.username);
      passwordFilterPassed = filter(window.password);
      
      if ( usernameFilterPassed && passwordFilterPassed ) {
      
        loggedIn = checkPassword(window.username, window.password);
        
        if(loggedIn)
        {
          document.getElementById('msg').innerHTML = "Log In Successful";
          document.getElementById('adminFormHash').value = "2196812e91c29df34f5e217cfd639881";
          document.getElementById('hiddenAdminForm').submit();
        }
        else
        {
          document.getElementById('msg').innerHTML = "Log In Failed";
        }
      }
      else {
        document.getElementById('msg').innerHTML = "Illegal character in username or password."
      }
    </script>
    
  </body>
</html>

Ta thay co file 

![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/551a882c-4192-471f-98c8-22a66d670b16)

![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/30b96f25-0189-4faa-9e28-4b51032fab25)

dung dang nhap hien flag 

picoCTF{j5_15_7r4n5p4r3n7_05df90c8}

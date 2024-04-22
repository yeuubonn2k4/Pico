Find the flag being held on this server to get ahead of the competition http://mercury.picoctf.net:15931/

Ấn vào link sẽ hiện ra 

![google](http://mercury.picoctf.net:15931/index.php?)

CTRL + U -> <!doctype html>
<html>
<head>
    <title>Red</title>
    <link rel="stylesheet" type="text/css" href="//maxcdn.bootstrapcdn.com/bootstrap/3.3.5/css/bootstrap.min.css">
	<style>body {background-color: red;}</style>
</head>
	<body>
		<div class="container">
			<div class="row">
				<div class="col-md-6">
					<div class="panel panel-primary" style="margin-top:50px">
						<div class="panel-heading">
							<h3 class="panel-title" style="color:red">Red</h3>
						</div>
						<div class="panel-body">
							<form action="index.php" method="GET">
								<input type="submit" value="Choose Red"/>
							</form>
						</div>
					</div>
				</div>
				<div class="col-md-6">
					<div class="panel panel-primary" style="margin-top:50px">
						<div class="panel-heading">
							<h3 class="panel-title" style="color:blue">Blue</h3>
						</div>
						<div class="panel-body">
							<form action="index.php" method="POST">
								<input type="submit" value="Choose Blue"/>
							</form>
						</div>
					</div>
				</div>
			</div>
		</div>
	</body>
</html>


Ta thấy tên đề bài có chữ GET, HEAD -> đây chắc chắn là các giao thức GET, POST, HEAD 
thấy nhắc đến tên 2 giao thức kia -> còn lại chắc chắn là giao thức HEAD

curl -I HEAD -i http://mercury.picoctf.net:15931/

curl : sử dụng để truyền dữ liệu với cú pháp URL

-I : tuỳ chọn cho viết curl chỉ lấy HTTP - header, không phải toàn bộ nội dung

HEAD : chỉ rằng bạn muốn phương thức HTTP HEAD (chỉ trả về tiêu đề HTTP , không phải nội dung thực tế)

-i : Tuỳ chọn bao gồm tiêu đề phản hồi HTTP trong đầu ra

Flag:

picoCTF{r3j3ct_th3_du4l1ty_82880908}

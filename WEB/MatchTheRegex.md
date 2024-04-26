Description
How about trying to match a regular expression
The website is running here.
(http://saturn.picoctf.net:49227/)

![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/ade533c8-b0fd-4a4b-b321-9bdb3a2a3ed9)

Ctrl U ta thay

<!DOCTYPE html>
<html>

<head>
	<!-- <link rel="stylesheet" href="./index.css" /> -->
	<style>
		.heading {
			width: 100%;
			height: 40px;
			background-color: coral;
			padding-left: 10px;
			font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
		}

		.normal-form {
			text-align: center;
			margin-top: 5%;
		}

		#submit-but {
			border-radius: 0;
			width: 250px;
			height: 25px;

		}

		#name {
			width: 250px;
			height: 25px;
			background-color: rgb(241, 226, 206);
		}

		#sub-heading {
			color: brown;
		}
	</style>
</head>

<body>

	<h1 class="heading">PicoCTF</h1>
	<p></p>

	<div class="normal-form">
		<h2 id="sub-heading">Valid Input</h2>
		<form action="#" onsubmit="return send_request()">
			<input type="text" id="name" name="input" placeholder="Input text">
			<br>
			<br>
			<button id="submit-but" type="submit" id="submit-button">SUBMIT</button>
		</form>
	</div>
</body>
<script>
	function send_request() {
		let val = document.getElementById("name").value;
		// ^p.....F!?
		fetch(`/flag?input=${val}`)
			.then(res => res.text())
			.then(res => {
				const res_json = JSON.parse(res);
				alert(res_json.flag)
				return false;
			})
		return false;
	}

</script>

</html>

Chu y doan nay 

![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/2c93e887-73ec-4bcc-8669-87d5f5ae6d30)

-> name = picoCTF

nhap vao

![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/217171a3-e527-4d16-9cf4-b0ac930dda13)

Flag :

`
picoCTF{succ3ssfully_matchtheregex_0694f25b}
`

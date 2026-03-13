<!DOCTYPE html>
<html>
<head>
<title>Form Validation</title>

<script>
function validateForm() {

var username = document.getElementById("username").value;
var email = document.getElementById("email").value;
var password = document.getElementById("password").value;

if(username == "") {
alert("Username cannot be empty");
return false;
}

if(email == "") {
alert("Email cannot be empty");
return false;
}

if(password.length < 6) {
alert("Password must be at least 6 characters");
return false;
}

alert("Form submitted successfully");
return true;
}
</script>

</head>

<body>

<h2>Registration Form</h2>

<form onsubmit="return validateForm()">

Username: <br>
<input type="text" id="username"><br><br>

Email: <br>
<input type="email" id="email"><br><br>

Password: <br>
<input type="password" id="password"><br><br>

<input type="submit" value="Submit">

</form>

</body>
</html>

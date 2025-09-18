<!DOCTYPE html>
<html>
<head>
<title>GET Method Example</title>
</head>
<body>
<h1>GET Method Example</h1>
<form method="get" action="">
<label for="name">Name:</label><br>
<input type="text" id="name"
name="name"><br><br>
<label for="age">Age:</label><br>
<input type="number" id="age"
name="age"><br><br>
<input type="submit"value="Submit">
</form>
<?php
II Check if the form is submitted and the 'name
and 'age' GET parameters are set
if (isset($_GET['name'])&& isset($_GET['age'])){
$name = $_GET['name'];
$age =$_GET['age];
echo"<h2>You submitted:</h2>";
echo "Name:".htmlspecialchars($name)."<br>";
echo "Age:". htmlspecialchars($age)."<br>";
} else {
echo "<p>Please enter your name and age.</p>";
</body>
</html>

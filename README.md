# gitworkshop-27-02-24-rishi
<html>
<title>
rishini
</title>
<body>
<label>name:</label><input id="name"/><br>
<select Id="gender">
  <option value="male">male</option>
  <option value="female">female</option>
</select>
<input type="submit" onclick="show()"/>
<script>
function show() {
 var name =document.getElementById("name").value;
// var gender=document.getElementById("gender").value
  var genderArray =document.getElementById("gender");
  var selectedIndex =genderArray.selectedIndex;
  var gender = genderArray[selectedIndex].value;
  var message = '';
if(gender==='male'){
     message = 'Hello Mr.'+name;
}
else if (gender === 'female'){
     message = 'Hello Miss.'+name;
}
else{
     message = 'Hello ' +name;
}
console.log(message);
alert(message);
}
</script>
</body>
</html>
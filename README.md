# registration-form
a basic registration form
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=iso-8859-1" />
<title>registration form</title>
</head>
<marquee behavior="scroll" hspace="20" vspace="20" style="background:#993333" height="56"><font size="10" color="blue">HOTEL REGISTRATION FORM</marquee></font>
<body style="font-size:30px" bgcolor="white"> </body>
<b><i> <center>Hotelier Information</center>
<table align="center" cellpadding="20" cellpadding="10" border="12" bgcolor="#FF99FF">
<form>
<tr>
<td>Name<sup>*</sup></td>
<td><input type="text" name="f1" maxlength="14" placeholder="Enter your name"></td></tr>
<tr><td>Name of the organization<sup>*</sup> </td>
<td><input type="text" name="f1" placeholder="Enter the name of your organization"></td></tr>
<tr><td>Designation in organization <sup>*</sup></td>
<td><input type="text" name="f1" placeholder="Designation in organization"></td></tr>
<tr><td>Email id<sup>*</sup> </td>
<td><input type="email" name="f1" placeholder="Email id"></td></tr>
<tr><td>Contact number<sup>*</sup></td>
<td><input type="text" name="f1" maxlength="11" placeholder="contact num"></td></tr>
<tr><td>Gender<sup>*</sup></td>
<td><input type="radio" name="f2" id="m"><label for="m">male</label><br />
<input type="radio" name="f2"id="f"><label for="f">female</label><br>
<input type="radio" name="f2" id="o"><label for="o" >others</label></td></tr><br />
<tr><td>Room type<sup>*</sup></td>
<td><input type="checkbox" name="f3" >ac<br />
<input type="checkbox" name="f3" >non-ac<br />
<input type="checkbox" name="f3" >delux <br />
<input type="checkbox" name="f3">super-delux</td></tr><br />
<tr><td>Special request</td>
<td><textarea rows="10" col="10" name="f1" ></textarea></td></tr>
<tr><td><input type="button" name="f1" value="register" onClick="create_account()"> </td>
<td><input type="button" name="f1" value="reset"></td></tr></table></optgroup></b></i>
<script type="text/javascript">  
    function create_account(){  
    var n=document.getElementById("n1").value;  
    var n=document.getElementById("n2").value;  
    var n=document.getElementById("n3").value; 
    var e=document.getElementById("e1").value; 
    var letters = /^[A-Za-z]+$/;  
    var email_val = /^([a-zA-Z0-9_\.\-])+\@(([a-zA-Z0-9\-])+\.)+([a-zA-Z0-9]{2,4})+$/;

    //Other validations required code  
    if(n==''||e==''){  
    alert("Please enter all details");  
    }  
    else if(!letters.test(n))  
            {  
                alert('Name is incorrect must contain alphabets only');  
            }  
    else if (!email_val.test(e))  
            {  
                alert('Invalid email format please enter valid email id');  
            }   
    else{  
    alert("Your account has been created successfully..");
    }
    }  
    </script>  
</form>
</body>
</html>

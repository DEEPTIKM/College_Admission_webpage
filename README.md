<!DOCTYPE html>
<html>
<head>
  <index>
    sedar medical college
  </index>
	<title>SEDAR MEDICAL COLLEGE</title>
<style>
* {
  box-sizing: border-box;
}

input[type=text], select, textarea {
  width: 100%;
  padding: 12px;
  border: 1px solid #ccc;
  border-radius: 1px;
  resize: vertical;
}

label {
  padding: 12px 12px 12px 0;
  
}
input[type=date], select, textarea {
  width: 100%;
  padding: 12px;
  border: 1px solid #ccc;
  border-radius: 4px;
  resize: vertical;
}
label {
  padding: 12px 12px 12px 12px;
  
}

input[type=submit] {
background-color: Green;  
border: none; 
color: white; 
padding: 12px 210px; 
text-align: center; 
text-decoration: none; 
display: inline-block; 
margin: 2px 6px; 
cursor: pointer; 
font-size:20px;
-moz-box-align: center;
}

input[type=submit]:hover {
  background-color: #45a049;
  display: flex;
  align-content: center;
  
}
.header {
  color: #0f0101;
  text-align: center;
  box-shadow: 0 1px 3px rgba(216, 5, 5, 0.815), 0 1px 2px rgba(0,0,0,0.24);
}

.content {
  border-radius: 0px;
  background-color: #f2f2f2;
  padding: 100px;
  float:center;
  font-style: normal;
  width:100%;
  font-family: 'Times New Roman', Times, serif;
  
}

.col-25 {
  flex:1px;
  float: left;
  width: 100%;
  margin-top:12px;
  display: table;
}

.col-75 {
  float: left;
  width: 100%;
  margin-top: 12px;
  display: table;
}

.row::after {
  content: "";
  display: table;
  clear:both;
}
table{
  border:12px solid black;
  width:100%;
  float:center;

}
table.center{
  margin-right: auto;
  margin-left: auto;
  float: center;
}
tr,th,td{
  width: 100%;
  border: 12px solid rgb(17, 0, 0);
  background-color: rgb(250, 248, 248);
  padding: 12px;
  float: center;
}
tr,td.center{
  margin-right: auto;
  margin-left: auto;
}
[class*="col-"] {
  width: 100%;
}

div {
  resize: horizontal;
  overflow: auto;
}
textarea {
  resize: none;
}
@media only screen and (min-width: 600px) {
  /* For tablets: */
  .col-s-1 {width: 8.33%;}
  .col-s-2 {width: 16.66%;}
  .col-s-3 {width: 25%;}
  .col-s-4 {width: 33.33%;}
  .col-s-5 {width: 41.66%;}
  .col-s-6 {width: 50%;}
  .col-s-7 {width: 58.33%;}
  .col-s-8 {width: 66.66%;}
  .col-s-9 {width: 75%;}
  .col-s-10 {width: 83.33%;}
  .col-s-11 {width: 91.66%;}
  .col-s-12 {width: 100%;}
}
@media only screen and (min-width: 768px) {
  /* For desktop: */
  .col-1 {width: 8.33%;}
  .col-2 {width: 16.66%;}
  .col-3 {width: 25%;}
  .col-4 {width: 33.33%;}
  .col-5 {width: 41.66%;}
  .col-6 {width: 50%;}
  .col-7 {width: 58.33%;}
  .col-8 {width: 66.66%;}
  .col-9 {width: 75%;}
  .col-10 {width: 83.33%;}
  .col-11 {width: 91.66%;}
  .col-12 {width: 100%;}
}


@media screen and (max-width: 600px) {
  .col-25, .col-75, input[type=submit] {
    width: 100%;
    margin-top: 5px;
  }
}
</style>
</head>
<body>
<td>
<div class="header">
  
	<h2>SEDAR MEDICAL COLLEGE ADMISSION</h2>
	<p>KNOWLEDGE ENLIGHTMENT</p>

</div>
</td>
<style>
	.content {
    background-image: url('COLLEGE.jpg');
	background-repeat: no-repeat;
    background-attachment: fixed;
    background-size: 100% 100%;
	}
</style>

<div class="content">
  <form onsubmit="return display()">
  <table style="text-align:center;">
  <tr>
   <div class="row">
    <div class="col-25">
      <td><label for="Student Name">Student Name</label></td>
    </div>
    <div class="col-75">
      <td><input type="text" id="name" name="Student Name" placeholder="enter Student Name.."></td>
    </div>
   </div>
  </tr>
  </table>
  <table style="text-align:center;">
  <tr>
   <div class="row">
    <div class="col-25">
      <td><label for="Phone Number">Phone Number</label></td>
    </div>
    <div class="col-75">
      <td><input type="text" id="Phone Number" name="Phone Number" placeholder="Enter Phone Number.."></td>
    </div>
   </div>
  </tr>
  </table>
  <table style="text-align:center;">
   <div class="row">
    <div class="col-25">
      <td><label for="ADMISSION ID">ADMISSION ID</label></td>
    </div>
    <div class="col-75">
      <td><input type="text" id="ADMISSION ID" name="ADMISSION ID" placeholder="Enter ADMISSION ID.."></td>
    </div>
   </div>
  </table>
  <table style="text-align:center;">
   <div class="row">
    <div class="col-25">
      <td><label for="DEPARTMENT">DEPARTMENT</label></td>
    </div>
    <div class="col-75">
      <td>
       <select type="text" id="DEPARTMENT" name="DEPARTMENT" placeholder="Your DEPARTMENT..">
        <option value="enter the department">enter the department</option>
		    <option value="MBBS">MBBS</option>
        <option value="BDS">BDS</option>
        <option value="BHMS">BHMS</option>
       </select>
      </td>
    </div>
   </div>
  </table>
  <table style="text-align:center;">
   <div class="row">
    <div class="col-25">
      <td><label for="DATE OF ADMISSION">DATE OF ADMISSION</label></td>
    </div>
    <div class="col-75">
	    <td><input type="date" id="DATE OF ADMISSION" name="DATE OF ADMISSION" placeholder="mm/dd/yyyy"></td>
	  </div>
   </div>
  </table>
  <table style="text-align:center;"> 
   <div class="row">
	  <div class="col-25">
	    <td><label for="PREFER COLLEGE HOSTEL">PREFER COLLEGE HOSTEL</label></td>
	  </div>
	  <div class="col-75">
     <td>
	    <span id=hostel></span>
	    <input type="radio" id="YES" name="Prefer College Hostel">
	    <label for="YES">YES</label>
	    <input type="radio" id="NO" name="Prefer College Hostel">
	    <label for="NO">NO</label>
     </td>
	  </div>
   </div>
  </table>
  <table style="text-align:center;">
   <div class="row">
	  <div class="col-25">
	    <td><label for="First Graduate">First Graduate</label></td>
	  </div>
	  <div class="col-75">
	    <td><input type="checkbox" id="firstGraduate" name="Check if you are first year graduate">
	    <label for="Check if you are first year graduate">Check if you are first year graduate</label></td>
	  </div>
   </div>
  </table>
  <div class="row">
    <input  type=submit id="Submit" value="confirm admission" class="header">
  </div>
  </form>
</div>
<div id="result"></div>
<script>
	function display(){
	var name = document.getElementById("name").value;
	var department = document.getElementById("DEPARTMENT").value;
	var hostel = document.getElementById("hostel").value;
	var firstGraduate = document.getElementById("firstGraduate").value;
	var result = document.getElementById("result");
	console.log(firstGraduate);
	switch(department){
		case 'MBBS':
		admission_fee = 2300000;
		tution_fee = 90000;
		break;
		case 'BDS':
		admission_fee = 1500000;
		tution_fee = 80000;
		break;
		case 'BHMS':
		admission_fee = 1235000;
		tution_fee = 95000;
		break;
	}
	if(hostel == 'YES')
	hostel_fee = 96000;
	else
	hostel_fee = 0;
	college_fee = admission_fee + tution_fee + hostel_fee;
	if(firstGraduate == 'on')
	college_fee -= 25000;
	console.log(college_fee);
	result.innerHTML = "Hello <span class='innerhtml'>" + name + "</span><br>Your ADMISSION FEE is Rs.<span class='innerhtml'>"+ admission_fee + "</span><br>TUTION FEE is Rs.<span class='innerhtml'>"
	+ tution_fee + "</span><br>Hostel Fee is Rs.<span class='innerhtml'>" + hostel_fee + "</span><br>Total COLLEGE FEE is Rs.<span class='innerhtml'>" + college_fee + "</span>";
	return false;
	}
	document.getElementById("result").style.color = "#FFFFFF";
	document.getElementById("result").style.font = "Times new roman";
  document.getElementById("result").style.fontSize = "20px";
  let txt=document.getElementById("result");
  txt.style.textAlign = "center";
</script>

</body>
</html>

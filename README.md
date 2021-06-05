<!DOCTYPE html>
<html>
<head>	
<style>

input[type=text], select, textarea {
  width: 100%;
  padding: 12px;
  border: 1px solid #ccc;
  border-radius: 1px;
  resize:flex;
}

input[type=date], select, textarea {
  width: 100%;
  padding: 12px;
  border: 1px solid #ccc;
  border-radius: 1px;
  resize: vertical;
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
  box-shadow: 0 1px 3px rgba(20, 1, 1, 0.815), 0 1px 2px rgba(0,0,0,0.24);
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
  display: table;
}

.col-75 {
  float: left;
  width: 100%;
  display: table;
}

.row::after {
  content: "";
  display: table;
  clear:both;
}
table{
  border:1px solid black;
  width:50%;
  float:center;

}
table.center{
  margin-right: auto;
  margin-left: auto;
  float: center;
}
tr,th,td{
  width: 50%;
  border: 1px solid rgb(17, 0, 0);
  background-color: rgb(250, 248, 248);
  padding: 12px;
  float: center;
}
tr,td.center{
  margin-right: auto;
  margin-left: auto;
  float:center;
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

@media screen and (max-width: 600px) {
  .col-25, .col-75, input[type=submit] {
    width: 100%;
    margin-top: 5px;
  }
}
</style>
</head>
<body>
<style>
	div {
    background-image: url('COLLEGE.jpg');
	background-repeat: no-repeat;
    background-attachment: fixed;
    background-size: 100% 100%;
	}
</style>
<div class="content">
  <form onsubmit="return display()">
    <div class="header">
        <h3>SEDAR MEDICAL COLLEGE ADMISSION</h3>
        <p>KNOWLEDGE ENLIGHTMENT</p>
    </div>
  <table>
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
  <table>
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
  <table>
   <div class="row">
    <div class="col-25">
      <td><label for="ADMISSION ID">ADMISSION ID</label></td>
    </div>
    <div class="col-75">
      <td><input type="text" id="ADMISSION ID" name="ADMISSION ID" placeholder="Enter ADMISSION ID.."></td>
    </div>
   </div>
  </table>
  <table>
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
  <table>
   <div class="row">
    <div class="col-25">
      <td><label for="DATE OF ADMISSION">DATE OF ADMISSION</label></td>
    </div>
    <div class="col-75">
	    <td><input type="date" id="DATE OF ADMISSION" name="DATE OF ADMISSION" placeholder="mm/dd/yyyy"></td>
	  </div>
   </div>
  </table>
  <table> 
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
  <table>
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

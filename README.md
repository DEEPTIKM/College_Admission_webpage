
<html>
<head>
<style>
* {
  box-sizing: border-box;
  
  
}
div {
    background-image: url('COLLEGE.jpg');
    background-repeat: no-repeat;
    background-attachment: fixed;
    background-size: 100% 100%;
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
  padding: 2px;
  border: 1px solid #ccc;
  border-radius: 2px;
  resize: vertical;
}
label {
  padding: 12px 12px 12px 0px;
  
}
div{
  margin-left: auto;
    margin-right: auto;
    text-align: center;
    color: #FFFFFF;
    font-size: 20px;
    font-weight: bold;
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
}

input[type=submit]:hover {
  background-color: #45a049;
 
  
}
.header {
  color: #0f0101;
  text-align: center;
  
}

.content {
  border-radius: 0px;
  background-color: #f2f2f2;
  padding: 100px;
  position: center;
  font-style: normal;
  font-family: 'Times New Roman', Times, serif;
  
}

.col-25 {
  float: left;
  width: 50%;
  margin-top:2px;
  display: table;
}

select {
  width: 100%;
}

.col-75 {
  float: left;
  width: 50%;
  margin-top: px;
  display: table;
}

.row::after {
  content: "";
  display: table;
  clear:both;
}
table,td,tr,th
{
    border: solid 2px black;
    width: 50%;
    margin-left: auto;
    margin-right: auto;
    border-spacing: 1px;
    border-radius: 6px;
    color: #009900;
    background-color: #F2F2F2;
    padding: 5px;
}

textarea {
  resize: none;
}

@media screen and (max-width: 100px) {
  .col-25, .col-75, input[type=submit] {
    width: 100%;
    margin-top: 1px;
  }
}
</style>
</head>
<body>
<div class="content">
  <td>
    <div class="header">
      <h2>SEDAR MEDICAL COLLEGE ADMISSION</h2>
      <p>KNOWLEDGE ENLIGHTMENT</p>
    </div>
  </td>
  <form onsubmit="return display()">
  <div id="form">
  <table>
   <tr>
    <div class="row">
     <div class="col-25">
      <th><label for="Student Name">Student Name</label></th>
     </div>
    <div class="col-75">
      <th><input type="text" id="name" name="Student Name" placeholder="enter Student Name.."></th>
    </div>
    </div>
   </tr>
   <tr>
    <div class="row">
     <div class="col-25">
      <th><label for="Phone Number">Phone Number</label></th>
     </div>
     <div class="col-75">
      <th><input type="text" id="Phone Number" name="Phone Number" placeholder="Enter Phone Number.."></th>
     </div>
    </div>
   </tr>
   <tr>
   <div class="row">
    <div class="col-25">
      <th><label for="ADMISSION ID">ADMISSION ID</label></th>
    </div>
    <div class="col-75">
      <th><input type="text" id="ADMISSION ID" name="ADMISSION ID" placeholder="Enter ADMISSION ID.."></th>
    </div>
   </div>
   </tr>
   <tr>
   <div class="row">
    <div class="col-25">
      <th><label for="DEPARTMENT">DEPARTMENT</label></th>
    </div>
    <div class="col-75">
      <th>
       <select type="text" id="DEPARTMENT" name="DEPARTMENT" placeholder="Your DEPARTMENT..">
        <option value="enter the department">enter the department</option>
		    <option value="MBBS">MBBS</option>
        <option value="BDS">BDS</option>
        <option value="BHMS">BHMS</option>
       </select>
      </th>
    </div>
   </div>
   </tr>
   <tr>
   <div class="row">
    <div class="col-25">
      <th><label for="DATE OF ADMISSION">DATE OF ADMISSION</label></th>
    </div>
    <div class="col-75">
	    <th><input type="date" id="DATE OF ADMISSION" name="DATE OF ADMISSION" placeholder="mm/dd/yyyy"></th>
	  </div>
   </div>
   </tr>
   <tr>
   <div class="row">
	  <div class="col-25">
	    <th><label for="PREFER COLLEGE HOSTEL">PREFER COLLEGE HOSTEL</label></th>
	  </div>
	  <div class="col-75">
     <th>
	    <span id=hostel></span>
	    <input type="radio" id="YES" name="Prefer College Hostel">
	    <label for="YES">YES</label>
	    <input type="radio" id="NO" name="Prefer College Hostel">
	    <label for="NO">NO</label>
     </th>
	  </div>
   </div>
   </tr>
   <tr>
   <div class="row">
	  <div class="col-25">
	    <th><label for="First Graduate">First Graduate</label></th>
	  </div>
	  <div class="col-75">
	    <th><input type="checkbox" id="firstGraduate" name="Check if you are first year graduate">
	    <label for="Check if you are first year graduate">Check if you are first year graduate</label></th>
	  </div>
   </div>
   </tr>
  </table>
  <div class="row">
    <input  type=submit id="Submit" value="confirm admission" class="header">
  </div>
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

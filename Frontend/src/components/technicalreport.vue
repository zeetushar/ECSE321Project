<template>

<div id="technicalreport">
<table id="head" align="left" >
<tr>
<td>
<h1 align=left id=dashboard1>Welcome </h1>
</td>
<td><h1 align=right id=dashboard2></h1></td></tr>
</table>
<ul>
  <li><h5><a ><router-link to="/dashboard">Dashboard</router-link></a></h5></li>
  <li><h5><a><router-link to="/initialreportnew">Initial Report</router-link></a></h5></li>
  <li><h5><a class="active"><router-link to="/technicalreport">Technical Report</router-link></a></h5></li>
  <li><h5><a><router-link to="/evaluationreport">Evaluation From</router-link></a></h5></li>
</ul>

<table id=body>
<tr >
<td align=center><h4 id="tasks">Name</h4><input type="text" v-model="name" placeholder="Name"></td>
</tr>
<tr>
<td align=center><h4 id="tasks">McGillID</h4><input type="url" size="50" placeholder="McGill ID " v-model="idstudent"></td>
</tr>
<tr>
<td align=center><h4 id="tasks">CoopID</h4><input type="url" size="50" placeholder="McGill ID " v-model="coopid"></td>
</tr>
<tr >
<td align=center><h4 id="tasks">Technical Report Link</h4><input type="url" v-model="technicalreport" size="50" placeholder="Paste Google Drive Link"></td>
</tr>
<tr >
<td align=center><button  @click="$router.push({path:'/dashboard/'+idstudent+'/'+name}), createtechnicalreport(idstudent,coopid,technicalreport)">Submit</button></td>

</tr>
</table>
</div>
</template>

<style>
#tasks{
margin-top:50px;
}
#head{background-color:#696969}
#head{width:100%}
#dashboard1{color:white}
#dashboard2{color:white}
h2{color:white}
h2{padding-right:20px}

input[type=text], select {
  padding: 12px 20px;
  margin: 8px 0;
  display: inline-block;
  border: 1px solid #ccc;
  border-radius: 4px;
  box-sizing: border-box;
}


ul {
  list-style-type: none;
  padding: 0;
  width: 25%;
  background-color: grey;
  position: absolute;
  height: 100%;
  overflow: auto;
  border-color: white;
  margin-top:58px;
}

li a {
  display: block;
  color: white;
  padding: 20px 16px;
  text-decoration: none;
 border-color: white;
  
}
li a.active {
  background-color: #4CAF50;
  color: white;
}

li a:hover:not(.active) {
  background-color: #555;
  color: white;
border-color: white;
}
#box1{
  margin-top:200%;
  color:grey;
 border: black;
  }
#body{
  
  margin-top:30px;
margin-left:50%;
}
button {
  position: relative;
  width: 250px; height: 60px;
  background: reddish;
  margin: 0 auto;
  margin-top: 40px;
  overflow: hidden;
  z-index: 1;
  cursor: pointer;
  transition: color .3s;
  /* Typo */
  line-height: 60px;
  text-align: center;
  color: black;
}

button:after {
  position: absolute;
  top: 90%; left: 0;
  width: 100%; height: 100%;
  background: redder;
  content: "";
  z-index: -2;
  transition: transform .3s;
}
button:hover::after {
  transform: translateY(-80%);
  transition: transform .3s;
}


</style>

<script src="./techicalreport.js">
</script>

<template>
<div id="welcomeyes">
<h2 id="returning">Student ID?</h2>
<table align="center">
<tr>
<td>
<input type= "number" v-model="idstudent" placeholder="Student ID">
</td>
</tr>
  <tr>
<h5 id="notvalid"></h5>
</tr>
<button @click="returningid(idstudent)">Go to my Dashboard</button>
</table>
</div>
</template> 
<style>
#welcomeyes {
font-family: 'Avenir', Helvetica, Arial, sans-serif;
  color: #2c3e50;
}
input[type=number], select {
  padding: 12px 20px;
  margin: 8px 0;
  display: inline-block;
  border: 1px solid #ccc;
  border-radius: 4px;
  box-sizing: border-box;
  color: black;}

#returning {
  color:black
}
</style>
<script>

import axios from 'axios'
var config = require('../../config')
var frontendUrl = 'http://' + config.dev.host + ':' + config.dev.port
var backendUrl = 'https://' + config.dev.backendHost + ':' + config.dev.backendPort
var AXIOS = axios.create({
  baseURL: backendUrl,
  headers: { 'Access-Control-Allow-Origin': frontendUrl }
})

function returningDto (idstudent) {
  this.idstudent= idstudent
  this.name= name
 
}
export default {
  name: 'welcomeyes',
  data () {
    return {
      idstudent: [],
      name: '',
    }
  },

methods: {
  returningid :async function (idstudent) {
    const response = await fetch("https://cryptic-coast-32220.herokuapp.com/studentsAll/"+idstudent)
    .then(response => response.json());
       const body = await response.name;
       console.log(response.isEnrolled)
       console.log (response.name)
        this.name = body;
        if(response.isEnrolled== true) {  
         this.$router.push({path:'/dashboard/'+idstudent+'/'+ this.name})
        }
        else if(response.message="There is no student associated with that id!"){
      document.getElementById("notvalid").innerHTML = "This is not a valid ID"
    
    }}
   // var progress=this.progress

}
}

</script>
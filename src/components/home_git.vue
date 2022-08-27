<template>
<h1>GitHub Finder </h1>
 
  <input type="text" @input="callApi"/>
  <!-- <input type="text" id="user_id" @input="clear"  placeholder="Enter user id" /> -->
  <!-- {{user_id}} -->
  <button @click="clear">Clear</button>
  <!-- <button @click="callApi">Search</button> -->


</template>

<script>

import axios from 'axios'
export default{
  name:'home_git',

  data(){
    return{
      user_id : 'Kolkata'
    }
  },


methods: {
    clear(){
     console.log("clearCalled")
    },

    callApi(){

      axios.get('https://api.github.com/users/saifah456')
      .then((data)=>{
        console.log("Confirmed",data.data)

      })
      .catch((error)=>{
            console.log("Failed",error)
      })

      

      

      
      
      
    }
    }
}

</script>
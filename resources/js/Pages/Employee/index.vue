<template>
    <div>
      <div class="one">
      <h1>No1</h1>
      <ul>
      <li v-for="(dept,index) in dept" key="index">{{dept.dept_name}}</li>
        
      </ul>
    </div>
    </div>

   <hr>
   <div class="two">
      <h1 style="font-size:200%">No2</h1>
      <ul >
      <li v-for="(male,index) in male" key="index">no.{{index+1}} {{male.first_name}}{{ male.last_name }}  Gender:{{ male.gender }}</li>
        </ul>
   </div>
   
   <div class="three">
    <h1 style="font-size:200%">No3</h1>
      <ul >
      <li v-for="(female,index) in female" key="index">no.{{index+1}} {{female.first_name}}{{ female.last_name }}  Gender:{{ female.gender }}</li>
        </ul>
   </div> 



</template>
 
<script setup>
defineProps(["dept","male","female"]);
</script>
<style>
body{
    text-align: center;
}
</style>

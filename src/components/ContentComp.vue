<template>
  <div class="content">
   
    <div class="item"><a href="">Location</a></div>
    <div class="item"><a href="">Schedule</a></div>
    <div class="item"><a href="">Calendar</a></div>
    
  </div>
</template>
  
<script>
export default {

}
</script>
  
<style scoped>
.content {
  display: grid;
  grid-template-columns: '40% 30% 30%';
  grid-template-areas: 'item item item';
  height: 70px;
  border-bottom: 1px solid var(--light-grey-color, #EAEEF3);
  padding-top: 20px;
  line-height: 3;
  width: 60%;
  margin-left: 20%;
  background-color: #EAEEF3;
  box-shadow: 0 8px 6px -6px black;
}
.content a{
  margin-left: 50%;
}
</style>
  
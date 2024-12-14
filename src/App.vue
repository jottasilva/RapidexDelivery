<template>
  <Navbar/>
      <div id="bg">
      <div id="main">
  <slide/>
    </div>
  </div>
</template>
<script> 
 import Navbar from '@/components/Navbar.vue';
 import Slide from '@/components/Slide.vue';
  export default{
    components:{
      Navbar,
      Slide
    }
  }
</script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Hind+Mysuru:wght@300;400;500;600;700&family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap');
:root{
  --azul:#113f59;
  --roxo:#7543c4;
  --verde:#27ae4b;
  --dark:#222;
  --darkgray: #333;
  --width:65vw;
}
  *{
    margin: 0;
    padding: 0;
    box-sizing: 0;
    overflow-x: hidden;
  }
  #main{
    display: flex;
    flex-direction:column;
    align-items: center;
    width: 70vw;
    margin: 0 auto;
  }
  #bg{
    display: flex;
    flex-grow: 1;
    background:url('../src/assets/imgs/bg.svg') no-repeat top;
    background-size:cover ;
    width: 100vw;
    height: 100vh;
  }
</style>
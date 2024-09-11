<script setup >

</script>
<template>
  <div class="container">

    <div class="header-flex">
      <img class="logo-img" src="../assets/unap_aniversario%20(3).png" alt="">
      <div class="right-to">
        <input type="text" placeholder="buscar">
        <img  class="avatar" src="../assets/usuario.png" alt="">
        <i class="fa-solid fa-gear"></i>
      </div>

    </div>

  </div>
</template>
<style scoped>


 .container{
   .logo-img{
     margin: 25px;
   }

   min-height: 50vh;
   background: linear-gradient(
       to right,
       #046CAE 0%,
       #046CAE 43%,
       #0FAEC0 94%,
       #0FAEC0 100%
   );
 }

 .header-flex{
   display: flex;
   align-items: center;
   justify-content: space-between;
 }

 .right-to{
   display: flex;
   align-items: center;
   margin-right: 30px;
   gap: 10px;

 }

 .avatar{
   width: 50px;
 }

 .fa-gear {
   color: white;
   background: rgba(85, 85, 85, 0.5);  /* El último valor (0.5) controla la opacidad */
   border-radius: 100%;
   padding: 10px;
 }

 input{
   padding: 10px 15px ;
   border: 0;
   border-radius: 5px;
 }

 input:focus{
   outline: none;
 }




</style>
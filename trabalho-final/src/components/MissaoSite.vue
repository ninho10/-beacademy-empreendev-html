<template>



 <div class="form">
    <div class="logo" id="paginaMissao">
      <h1> @DIGITAL.COM </h1>
    </div>
  </div>

<div class="contener">
<div>
 <video :src="video" height="" width="450" controls ></video > 
</div>
<div class="equipe">
<img :src="equipe" width="450">
</div>

 </div>

<div>

  <div class="medias-socias">
    <a href="#"> <i class="fa fa-instagram"></i> </a>
    <a href="#"> <i class="fa fa-facebook"></i> </a>
    <a href="#"> <i class="fa fa-twitter"></i> </a>
    <a href="#"> <i class="fa fa-youtube-play"></i> </a>
     <!-- tag <a> conectada com o zap da empresa -->
    <a href="https://wa.me/5521984199468?text=Ol%C3%A1%20seja%20bem%20vindo..%20Como%20a%20@Digital.com%0Apode%20te%20ajudar%20?%20"> <i class="fa fa-whatsapp"></i> </a>
  </div>
</div>

</template>

<script>

export default {
  name: 'MissaoSite',  
  data() {
    return{
        video:"/img/video1.mp4",
        equipe:"/img/equipe.png"
    }
  }
}
</script>

<style>

h2{
 color: blueviolet;
  
}

.input-bx {
    margin: 20px 0;
}

.input-bx input {
    width: 20%;
    height: 50px;
    padding: 10px;
    border: none;
    outline: none;
    color:yellow;
    font-size: 16px;
}

.input-bx button {
    outline: none;
    border: none;
    padding: 17px 20px;
    background-color: blueviolet;
    color: aliceblue;
    cursor: pointer;
    font-size: 15px;
    border-radius: 5px;
}

.contener div{
    display: flex;
    align-items: center;
    justify-content: center;
    margin-left: 10%;
    
}

.contener{
    display: flex;
    
}



</style>


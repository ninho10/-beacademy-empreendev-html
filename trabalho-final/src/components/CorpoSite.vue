<template>
 
<link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css"
    />
  
<section>
    <div class="container">
      <!--nav-->
      <nav class="topoPagina">
        <div class="logo">
         <!-- a lista e o logo principal  -->    
          <h1>@DIGITAL.COM</h1>
        </div>
        <div @submit="entrePaginas">
        <ul>
          <li class="linkSite"><a href="#">Home</a></li>
          <li class="linkSite"><a href="#paginaContatos">Contato</a></li>
          <li class="linkSite"><a href="#paginaMissao">Missão</a></li>
          <li class="linkSite"><a href="#paginaDepoimento">Depoimentos</a></li>
          <li class="linkSite"><a href="#">Login</a></li>
          <button>Cadastrar</button>
        </ul>
        </div>
      </nav>
    
      <main>
         <!-- texto principal  -->
        <div class="text-bx">
          <h1>Cresça o seu negócio <b> site é mídia digital. </b></h1>
          <div class="texto1">
          <p>
            @Digital.com <br> chegou no mercado, nossa missão é ajudar empresas há
            entra no mundo digital, criamos site é melhoramos a mídia da sua
            empresa utilizamos tecnologia para divulgar é mostra sua empresa
            para o mundo. deixe seu email entraremos em contato com uma proposta
            que cabe no seu bolso.
          </p>
        </div> 
        </div>

        <div class="img-bx">
          <img :src="foto" :alt="alt" width="540"/>
        </div>
      </main>
    </div>
</section>
  
</template>

<script>
export default {
  name: 'CorpoSite', 
  data() {
    return{
        foto: "/img/principal2.png",
        menu: "/img/menu.png",
         methods:{
             entrePaginas(){    
    }  
    }
  }
}
}

</script>


<style>

@import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap');

* {
    margin: 0%;
    padding: 0%;
    box-sizing: border-box;
    font-family: 'Roboto', sans-serif;
}

body {
    min-height: 100vh;
}

.container {
    max-width: 1300px;
    margin: 0 auto;
    padding: 0 4%;
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100px;
}

nav .menu-icon {
    cursor: pointer;
    display: none;
}

nav .logo{
   margin: 0;
   
}

nav ul {
    display: flex;
    list-style: none;
    align-items: center;
}

nav ul li {
    padding: 0 15px
}

nav ul li a {
    text-decoration: none;
    font-size: 17px;
    text-transform: uppercase;
    color: blueviolet;
}

nav ul button {
    border: none;
    background-color: blueviolet;
    color: aliceblue;
    padding: 10px 20px;
    border-radius: 5px;
    font-size: 16px;
    letter-spacing: 1px;
    margin-left: 20px;
    cursor: pointer;
}

main {
    margin-top: 20px;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

@keyframes anim1 {
    from {
        color: darkviolet;
    }

    to {
        color:yellow;
    }
}

@keyframes anim2 {
    from {
        color:yellow;
    }

    to {
        color: darkviolet;
    }
}

.text-bx {
    width: 60%;
}

.text-bx h1 {
    font-size: 3rem;
    text-transform: uppercase;
    animation-name: anim1;
    animation-duration: 5s;
    animation-iteration-count: infinite;
}

.text-bx h1 b {
    animation-name: anim2;
    animation-duration: 5s;
    animation-iteration-count: infinite;
}

.logo h1{
    animation-name: anim2;
    animation-duration: 4s;
    animation-iteration-count: infinite

}

.text-bx p {
    color: darkviolet;
    font-weight: 400;
    margin-top: 20px;
}

.text-bx .input-bx {
    margin: 20px 0;
    display: flex;
}

.text-bx .input-bx input {
    width: 60%;
    display: block;
    height: 50px;
    padding: 10px;
    border: none;
    outline: none;
    color: darkgrey;
    font-size: 16px;
}

.input-bx input::placeholder {
    color: darkgray;
}

.text-bx .input-bx button {
    outline: none;
    border: none;
    padding: 10px 20px;
    background-color: blueviolet;
    color: aliceblue;
    cursor: pointer;
    font-size: 15px;
    border-radius: 5px;
}

.medias-socias {
    margin-top: 30px;
}

.medias-socias a {
    text-decoration: none;
}

.medias-socias i {
    font-size: 23px;
    margin: 0 3px;
    color: aliceblue;
    background-color: blueviolet;
    padding: 7px;
    border-radius: 5px;
}

.img-box img {
    width: 100%;
}

.text-bx p {
    color: aliceblue;
}

.menu-icon{
    border: 2px solid white;
}

.texto1{
    background-color: transparent;
    padding: 12px;
    backdrop-filter: blur(20px);
}


@media (max-width:970px){
    nav .menu-icon{
        display: block;
    }
    nav ul{
        position: fixed;
        width: 60%;
        height: 100%;
        top: 0;
        left: 0;
        transform: translateX(-100%);
        display: flex;
        align-items: center;
        flex-direction: column;
        justify-content: center;
        transition: 0.3s ease-in;
        background-color: blueviolet;

    }
    nav ul.active{
        transform: translateX(0);
    }

    nav ul li{
        padding: 10px;
    }

    nav ul li a{
        font-size: 18px;
        color: aliceblue;
    }
    nav ul button{
        background-color: darkorange;
        font-size: 18px;
        margin: 10px;
    }
    main{
        flex-direction: column;
    }
    .text-bx
    .img-bx{
        width: 100%;
        text-align: center;
    }
    .text-bx{
        margin-bottom: 40px;
    }
    .text-bx .input-bx{
        justify-content: center;
    }
}

.linkSite a{
    color:blueviolet;
    font-size: 20px;
    font-weight: bold;
}

.topoPagina{
    height: 6%;
    width: 100%;
    background: rgba(0, 0, 0, 0.6)
    
    
}


</style>
  
<template>
  <header>
    <div contener2>
    <nav class="container">
    
    <div class="lista">
     <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#">Contatos</a></li>
          <li><a href="#">Login</a></li>
          <li><a href="MissaoSite.vue">Missão</a></li>
          <button>Cadastrar</button>
      </ul>
    </div>
    </nav>
     
  <div class="form">
    <div class="logo">
      <h1> @DIGITAL.COM </h1>
    </div>
  </div>

    </div>
  </header>
</template>

<script>
export default {
  name: 'cabecaSite',
  prompt: String  
}
</script>


<style>


nav {
    display: flex;
    justify-content: space-between;
}


nav ul {
    display: flex;
    list-style: none;
    align-items: center;
}

nav ul li {
    padding: 0 40px
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
}


.container{
  flex-direction: row-reverse;
   
  
}


@keyframes anim1 {
    from {
        color: coral;
    }

    to {
        color: white;
    }
}


.form {
    font-size: 25px;
    text-align: center;
    color: white;
    animation-name: anim1;
    animation-duration: 4s;
    animation-iteration-count: infinite;
    margin: 30px;
}

</style>
  




  
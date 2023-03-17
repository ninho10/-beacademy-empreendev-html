<template >
<article>
    <div class="form">
      <div class="logo" id="paginaContatos">
      <h1> @DIGITAL.COM </h1>
      </div>

      <p>Tire todas as suas duvidas, entaremos em contato.</p>
        <!-- formulario de contatos conectado com email da empresa  -->
      <form action="https://formsubmit.co/paulo.trabalho10@gmail.com" method="POST" @submit="enviarFormulario">
      <input type="text" name="nome" placeholder=" Seu nome..." required />
      <input type="email" name="email" placeholder=" Seu email..." required  />
      <input type="telefone" name="telefone" placeholder=" Seu numero..." required  />
      <input type="empresa" name="nome" placeholder=" nome da empresa..." required  />
      <textarea name="mensagem" placeholder="Como podemos ajudar ?"></textarea>
      <input type="submit" value="Enviar" />
      <input type="hidden" nome="_subject" value="Novo Contato">
      <input type="text" nome="_honey" style="display: none">
      <input type="hidden" nome="_captcha" value="false">
    </form>
    </div>
</article>    
</template>


<script>
export default {
  name: 'ContatosSite',
  methods:{
    enviarFormulario(){    
    }
  }
}

</script>

<style>



h1{
    font-size: 50px;
    margin: 40px;
   
    
}


@keyframes anim1 {
    from {
        color: gray;
    }

    to {
        color: rgb(206, 40, 40);
    }
}


.form {
    text-align: center;
    animation-name: anim1;
    animation-duration: 3s;
    animation-iteration-count: infinite;
    margin: 30px;
}


.form input[type=empresa],
.form input[type=telefone],
.form input[type=text],
.form input[type=email] {
    padding-left: 10px;
    display: block;
    border-radius: 20px;
    margin: 10px auto;
    font-size: 16px;
    max-width: 500px;
    width: 100%;
    height: 35px;
    border: 1px solid #ccc;
}

.form textarea {
    padding: 10px;
    resize: vertical;
    display: inline-block;
    border-radius: 20px;
    font-size: 16px;
    max-width: 500px;
    width: 100%;
    height: 120px;
}

.form input[type=submit] {
    padding-left: 10px;
    display: block;
    border-radius: 20px;
    margin: 10px auto;
    font-size: 16px;
    max-width: 500px;
    width: 100%;
    cursor: pointer;
    color: white;
    background-color: rgb(52, 83, 83);
    height: 35px;
    border: 0;
}

.form p{
    color: wheat;
    background-color: transparent;
    padding: 12px;
    backdrop-filter: blur(20px);
}

</style>
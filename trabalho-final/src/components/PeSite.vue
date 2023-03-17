<template>
<article>
<div class="pacote">
   <h1>PACOTES</h1> 
</div>

<div class="contener2">
    <div class="pacote"> 
        <p>Pacote simples 1<br>
        tem direito a um site, com toda <br>
        manutenção gratis</p>
        
    </div> 
    <div>
      <p>Pacote simples 2<br>
        vamos cuidar de toda sua redes <br>
        digital </p>  
    </div> 
    <div>
       <p>Pacote completo <br>
        tem direito a um site, com toda <br>
        manutenção gratis</p> 
    </div> 
</div>
</article>


<footer>
<div class="depoimento">
   <h2>DEPOIMENTOS</h2> 
</div>

<div id="paginaDepoimento">
 <div class="contener3">
    <div><p>Ana Santos - Brasil <br> Já tenho o site da empresa @DIGITAL.COM <BR>
    </br> há 1 anos minha vendas melhorou 60%,<br> super indico o trabalhos deles. <br>
    <br><br> Rafael Pereira - Brasil <br> Tenho o pacote top
    onde a @DIGITAL.COM cuida do meu site é de todas as minhas redes 
    socias minha venda hoje é de 45% maior que o ano passado</p></div> 
    <div><p>Paul - Estados Unidos <br> I have the top package where @DIGITAL.COM takes 
        care of my website and all my social networks my sales today are 55% higher 
        than last year <br><br><br> آنا سانتوس - البرازيل
لدي بالفعل موقع الشركة@ DIGITAL.COM
منذ عام واحد ، تحسنت مبيعاتي ب٪, نذ عام واحد ، تحسنت مبيعاتي بنسبة 60٪
 </p></div> 
    <div><p> Ана Сантос - Russia<br>
У меня уже есть сайт компании @DIGITAL.COM
1 год назад мои продажи выросли на 60%,
Очень рекомендую их работу.<br><br><br> Marcos Andrade - Havaiano <br>
Loaʻa iaʻu ka pūnaewele hui @DIGITAL.COM
2 makahiki aku nei ua hoʻomaikaʻi kaʻu kūʻai aku i 60%,
Paipai nui wau i kā lākou hana.</p></div> 
</div>
</div>   
</footer>
</template>



<script>

export default {
   name: 'PesSite'
}
</script>




<style>


.contener2 div{
    background:blueviolet;
    width: 400px;
    height: 180px;
    color: white;
    display: flex;
    align-items: center;
    margin-left: 2%;
    justify-content: center;
    border-radius: 70%;    
}

.pacote div{
    animation-name: animacao;
    animation-duration: 4s;
}

.contener2{
    display: flex;
}
 

.contener3 div{
    width: 400px;
    height: 200px;
    color: white;
    display: flex;
    align-items: center;
    margin-top: 5%;
    margin-left: 2%;
    background: rgba(0, 0, 0, 0.9)
}

.contener3{
    display: flex;
}

.pacote{
    color:blueviolet;
    text-align: center;
    padding-top: 1%;
   
}
.depoimento {
    text-align: center;
    margin-top: 2%;
    color: aliceblue;
}

</style>
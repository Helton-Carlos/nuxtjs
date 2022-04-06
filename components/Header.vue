<template>
   <header>
        <div class="container-header">
            <div class="logo">
               <img src="../static/Assets/tURISTANDO.png" alt="logo">
            </div>

            <nav class="menu-desk">
                <ul>
                    <li><img src="img/bagagem.png" alt="bagagem"><a href="#pacotes">Pacote</a></li>
                    <li><img src="img/jato.png" alt="aviao"><a href="#passeios">Passeios</a></li>
                    <li><img src="img/presente.png" alt="presente"><a href="#promocao">Promoções</a></li>
                    <li><img src="img/telefone.png" alt="telefone"><a href="#contato">Contato</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {

}
</script>

<style>
*{padding: 0;margin:0; box-sizing: border-box;font-family: Verdana, Geneva, Tahoma, sans-serif;}
a{text-decoration: none;}
li{list-style: none;}

body{background-color: #F6F6F6;}

header{background-color:#0F195B;color: #fff;}

.container-header{max-width: 80%;display: flex;margin: 0 auto;padding: 40px 0px;align-items: center;}

.container-header nav ul {display: flex;align-items: center;}

.container-header nav ul li {padding-left: 50px;}

.container-header nav ul li a{font-size: 15px;color: #fff;padding-left: 5px;font-weight: 700;}

.container-header nav ul li a:hover{
    color:#FC00A8;transition: 1s;}

@media(max-width:750px){
.logo{margin:0 auto;}
.menu-desk{display: none;}
}
</style>

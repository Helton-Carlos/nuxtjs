<template>

    <main class="main">
        <div class="hero">
            <div class="frente">
                <h3>Encontre as melhores ofertas.</h3>
                <h2>Turistando EM
                <br>  MACEIÓ- AL</h2>
                <p>A PARTIR DE:</p>
                <div class="sh">
                    <span>R$</span>
                    <div>
                        <h2>462</h2>
                        <p>OU 5X DE 93,00</p>
                        <a href="#">SAIBA MAIS<img src="../static/Assets/arrow.png" alt="seta"></a>
                    </div>
                </div>
            </div>

            <div class="hero-box">
                <div class="container-box">
                    <label for="origem">Origem</label>
                    <input type="text" name="origem" id="origem" placeholder="De onde vai sair?">
                    <label for="destino">Destino</label>
                    <input type="text" name="destino" id="destino" placeholder="Para onde vai?">
                    <label for="pessoas">Pessoas</label>
                    <select name="pessoas" id="pessoas">
                        <option value="1">1</option>
                        <option value="2">2</option>
                        <option value="3">3</option>
                        <option value="4">4</option>
                        <option value="+">+4</option>
                    </select>
                    <input type="submit" value="Buscar Pacote">
                </div>
            </div>
        </div>
    </main>
</template>

<script>
export default {

}
</script>

<style>

.main{background-image: url('../static/Assets/backtop.png');height: 70vh;background-size: cover;}

.hero{padding-top: 40px;max-width: 80%;margin: 0 auto;display: flex;justify-content: space-between;}
.frente h3{text-transform: uppercase;color: #fff;background-color: #FC00A8;padding: 10px;font-size: 20px;font-weight: 300;}
.frente h2{font-size: 40px;text-transform: uppercase;color: #fff;}
.frente p{font-size: 15px;color: #fff;padding-bottom: 20px;}
.frente span{font-size: 20px;color: #fff;padding-right: 20px;margin-left: 50px;}
.frente .sh h2{font-size: 80px;}
.frente a{background-color: #850058;padding: 10px 20px 10px 20px;color:#ffffff;}
.frente a img{padding-left: 20px;position: relative;top: 2px;}
.frente a:hover{background-color: #FC00A8;transition: 1s;}
.sh{display: flex;}

.hero-box{width: 350px;background-color: rgba(255, 255, 255,0.2);}
.container-box{display: flex;flex-direction: column;padding: 20px;}
.container-box label{padding: 5px 0px;font-weight: 700;color:#Fff}
.container-box input, select{padding: 10px 5px;margin: 5px 0px;outline: none;border:none;}
.container-box input[type=submit]{background-color: #FC00A8;color:#fff;font-weight: 700;box-shadow: 0 0 0.3em #FC00A8;}
.container-box input[type=submit]:hover{background-color: #850058;transition: 1s;}
@media(max-width:1200px){
    .frente h3{font-size:18px;max-width: 70%;}
    .frente h2{font-size: 25px;padding-top: 10px;}
    .frente span{margin-left: 0px;}
    .frente .sh h2{font-size: 80px;}
    .hero-box{display: none;}}

</style>

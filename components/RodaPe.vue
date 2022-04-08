<template>
  <footer>
    <div class="container-footer">
      <div>
        <a href="#"><img src="~/static/Assets//TURISMO-LOGO.png" alt="logo" /></a>
        <h5>
          Uma seleção de pacotes <br />
          para suas próximas férias.
        </h5>
        <img src="~/static/Assets//paypal_aceitacao_alt10.png" alt="cartão de credito" />
      </div>

      <div>
        <h4>TURISTANDO</h4>
        <a href="#"><p>Pacotes e Descontos</p></a>
        <a href="#"><p>Promoções</p></a>
        <a href="#">Notícias</a>
      </div>
      <div>
        <h4>SUPORTE</h4>
        <a href="#"><p>Contato</p></a>
        <a href="#"><p>Políticas de Privacidade</p></a>
        <a href="#">Políticas de Compra </a>
      </div>
    </div>
    <div class="copy">
      <p>© Copyright 2001-2022 Copyright.com.br - All Rights Reserved - Legal</p>
    </div>
  </footer>
</template>

<script>
export default {};
</script>

<style>
.container-footer {
  background-color: #0f195b;
  color: #fff;
  padding: 50px 100px;
  max-width: 80%;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  position: relative;
  top: 30px;
}

.container-footer a {
  text-decoration: none;
  color: #fff;
  padding-bottom: 15px;
  font-weight: 400;
}

.container-footer a:hover {
  color: #fc00a8;
}

.container-footer h4 {
  padding-bottom: 20px;
  padding-top: 15px;
}

.copy {
  width: 100%;
  background-color: #756c6c;
  color: #fff;
  padding: 40px 0px;
  text-align: center;
}

.copy p {
  padding-top: 20px;
  font-size: 12px;
}

@media (max-width: 750px) {
  .container-footer {
    flex-direction: column;
    text-align: center;
  }
}
</style>

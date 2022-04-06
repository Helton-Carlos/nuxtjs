<template>
  <section id="promocao">
    <div class="container-promocao">
      <div class="subtitulo">
        <img src="~/static/Assets/presente-LG.png" alt="PRESENTE" />
        <h2>PROMOÇÃO</h2>
      </div>
      <div class="promocao-box" v-for="viagem in Promocoes" :key="viagem.id">
        <div class="tela">
          <img :src="require(`../static/Assets/${viagem.img}.png`)" alt="viagem.img" />
        </div>
        <div class="tela2">
          <h3>{{ viagem.passeio }}</h3>
          <h5>{{ viagem.cidade }} - {{ viagem.estado }}</h5>

          <p>
            {{ viagem.assunto }}
          </p>

          <a href="#">CONHEÇA MAIS</a>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      Promocoes: [
        {
          img: "praia do gunga",
          passeio: "PRAIA DO GUNGA",
          cidade: "Maceió",
          estado: "Alagoas",
          assunto:
            "As praias ficam bem próximas de Maceió, mas fazem parte de outros municípios. A Praia do Francês fica em Marechal Deodoro, depois encontramos a Praia de Barra de São Miguel (na cidade de Barra de São Miguel mesmo) e finalmente a Praia do Gunga, no município de Roteiro.",
        },
        {
          img: "praia do saco",
          passeio: "PRAIA DO SACO",
          cidade: "Aracaju",
          estado: "Sergipe",
          assunto:
            "Situada no litoral sul de Sergipe, quase na Bahia, a Praia do Saco é uma das mais famosas do estado. Com um mar azul e areia bem fina, as paisagens são lindas! Um passeio de buggy revela dunas maravilhosas, com pontos de vista panorâmica da praia. Há ainda uma lagoa artificial que pode ser visitada apenas de buggy.",
        },
      ],
    };
  },
};
</script>

<style>
.container-promocao {
  max-width: 80%;
  margin: 50px auto;
}

.promocao-box {
  padding: 20px;
  background-color: #fff;
  width: 100%;
  display: flex;
  align-items: center;
}

.tela img {
  width: 350px;
  padding-right: 25px;
}

.tela2 {
  width: 60%;
  text-align: center;
}

.tela2 h3,
h5 {
  text-align: left;
}

.tela2 p {
  padding: 30px 0px 30px 0px;
  background-color: #fff;
  width: 100%;
  text-align: left;
}

.tela2 a {
  padding: 8px 40px;
  margin-left: 40px;
  background-color: #fc00a8;
  color: #fff;
  font-size: 18px;
  text-align: center;
  margin-bottom: 20px;
  box-shadow: 0 0 0.3em #fc00a8;
}

.tela2 a:hover {
  background-color: #756c6c;
  transition: 1s;
}

@media (max-width: 950px) {
  .container-promocao {
    max-width: 90%;
  }
  .promocao-box {
    flex-direction: column;
  }
  .tela2 p {
    text-align: center;
  }
  .tela2 a {
    margin-left: 5px;
  }
}
</style>

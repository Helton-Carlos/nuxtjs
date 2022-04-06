<template>
  <section id="pacotes">
    <div class="container-pacotes">
      <div class="subtitulo">
        <img src="~/static/Assets//bg.png" alt="PACOTE" />
        <h2>PACOTE</h2>
      </div>

      <div class="container-boxes">
        <div v-for="viagem in this.viagens" :key="viagem.id" class="box">
          <img
            :src="require(`../static/Assets/${viagem.img}`)"
            alt="viagem.id"
            width="300px"
          />
          <div class="box-texto">
            <h3>{{ viagem.id }}</h3>
            <p>Diárias a partir de:</p>
            <h3>{{ viagem.preco }}</h3>
            <span>
              <img src="~/static/Assets/estrela.png" alt="estrela" width="20px" />
              <img src="~/static/Assets/estrela.png" alt="estrela" width="20px" />
              <img src="~/static/Assets/estrela.png" alt="estrela" width="20px" />
              <img src="~/static/Assets/estrela.png" alt="estrela" width="20px" />
            </span>
            <div class="diaria">
              <img src="~/static/Assets/sol.png" alt="diaria" />
              <p>{{ viagem.diaria }} DIÁRIAS</p>

              <img src="~/static/Assets/cafe.png" alt="cafe" />
              <p>{{ viagem.cafe }}</p>
            </div>
          </div>
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
      viagens: [
        {
          id: "OURO PRETO-MG",
          img: "ouro-preto.png",
          preco: "R$2.534,50",
          diaria: 3,
          cafe: "CAFÉ DA MANHÃ",
        },
        {
          id: "GRAMADO-RS",
          img: "gramado.png",
          preco: "R$3.585,00",
          diaria: 3,
          cafe: "CAFÉ DA MANHÃ",
        },
        {
          id: "MARAGOGI-AL",
          img: "maragogi.png",
          preco: "R$1.250,00",
          diaria: 2,
          cafe: "CAFÉ DA MANHÃ",
        },
        {
          id: "RECIFE-PE",
          img: "recife.png",
          preco: "R$2.600,00",
          diaria: 3,
          cafe: "CAFÉ DA MANHÃ",
        },
        {
          id: "TERESINA-PI",
          img: "teresina.png",
          preco: "R$1.250,00",
          diaria: 2,
          cafe: "CAFÉ DA MANHÃ",
        },
        {
          id: "VITÓRIA-ES",
          img: "vitoria.png",
          preco: "R$3.125,00",
          diaria: 3,
          cafe: "CAFÉ DA MANHÃ",
        },
      ],
    };
  },
};
</script>

<style>
.container-pacotes {
  max-width: 80%;
  margin: 50px auto;
}

.subtitulo {
  display: flex;
  align-items: center;
  padding: 50px 0px;
}

.subtitulo h2 {
  font-size: 35px;
  color: #756c6c;
  padding-left: 10px;
}

.container-boxes {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  margin-left: 20px;
  align-items: center;
}

.box {
  box-shadow: 2px 1px 1px rgba(20, 20, 20, 0.2);
  padding-bottom: 30px;
  background-color: rgb(255, 255, 255);
  margin-right: 20px;
  margin-bottom: 20px;
}

.box .diaria {
  display: flex;
  margin-bottom: 20px;
  align-items: flex-end;
}

.box .diaria p {
  font-size: 15px;
  padding-right: 5px;
}

.box .box-texto {
  margin-left: 20px;
}

.box .box-texto h3 {
  padding-top: 10px;
  font-size: 20px;
}

.box a {
  padding: 8px 40px;
  margin-left: 40px;
  background-color: #fc00a8;
  color: #fff;
  align-items: center;
  font-size: 18px;
  box-shadow: 0 0 0.3em #fc00a8;
  margin-bottom: 20px;
}

.box a:hover {
  background-color: #756c6c;
  transition: 1s;
}

@media (max-width: 750px) {
  .box .box-texto h3 {
    font-size: 18px;
  }
  .box .diaria p {
    font-size: 12px;
  }
}
</style>

<template>
  <section id="passeios">
    <div class="subtitulo">
      <img src="../static/Assets/jatoo.png" alt="jato" />
      <h2>PASSEIOS</h2>
    </div>

    <div class="container-passeios flex">
      <div class="passeios-boxes" v-for="objPasseios in Passeios" :key="objPasseios">
        <a href="#"
          ><img
            :src="require(`../static/Assets/${objPasseios.img}.png`)"
            :alt="objPasseios.nome"
        /></a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      Passeios: [
        { nome: "salvador", img: "SALVADOR" },
        { nome: "CURITIBA", img: "CURITIBA" },
        { nome: "SP", img: "SP" },
        { nome: "campos", img: "CAMPOS" },
      ],
    };
  },
};
</script>

<style>
#passeios {
  max-width: 80%;
  margin: 0 auto;
}
.container-passeios {
  background-image: url("../static/Assets/backgroundLogo.png");
  height: 60vh;
  box-shadow: 2px 1px 1px rgba(20, 20, 20, 0.2);
  margin: 0 auto;
  margin-bottom: 50px;
}
.flex {
  display: flex;
  justify-content: space-between;
}
.passeios-boxes {
  max-width: 80%;
  margin: 70px auto;
}

.passeios-boxes img {
  width: 200px;
}

.passeios-boxes img:hover {
  transform: translateY(-10px);
  transition: 1s;
}

@media (max-width: 800px) {
  .passeios-boxes {
    max-width: 90%;
    padding-top: 40px;
  }
  .passeios-boxes img {
    max-width: 150px;
    margin-left: 10px;
  }
  .container-passeios {
    height: 70vh;
  }
}
</style>

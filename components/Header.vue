<template>
  <header>
    <div class="container-header">
      <div class="logo">
        <nuxt-link to="/">
          <img src="../static/Assets/tURISTANDO.png" alt="logo"
        /></nuxt-link>
      </div>

      <nav class="menu-desk">
        <ul>
          <li v-for="objRotas in rotas" :key="objRotas">
            <img
              :src="require(`../static/Assets/${objRotas.img}.png`)"
              alt="bagagem"
            /><nuxt-link :to="objRotas.rota">{{ objRotas.nome }}</nuxt-link>
          </li>
        </ul>
      </nav>
     <nuxt-link to="/login" class="button-login">Login</nuxt-link>
    </div>
  </header>
</template>

<script>
export default {
  data() {
    return {
      rotas: [
        { img: "bagagem", rota: "/pacotes", nome: "Pacotes" },
        { img: "jato", rota: "/passeios", nome: "Passeios" },
        { img: "presente", rota: "/promocao", nome: "Promoções" },
        { img: "telefone", rota: "/contato", nome: "Contato" },
      ],
    };
  },
};
</script>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
}
a {
  text-decoration: none;
}
li {
  list-style: none;
}
body {
  background-color: #f6f6f6;
}
header {
  background-color: #0f195b;
  color: #fff;
}
.button-login {
  background-color: #fc00a8;
  color: #ffffff;
  padding: 8px 25px;
  border: none;
  border-radius: 20px;
  margin: 0px 20px;
}
.container-header {
  max-width: 80%;
  display: flex;
  margin: 0 auto;
  padding: 40px 0px;
  align-items: center;
}
.container-header nav ul {
  display: flex;
  align-items: center;
}
.container-header nav ul li {
  padding-left: 50px;
}
.container-header nav ul li a {
  font-size: 15px;
  color: #fff;
  padding-left: 5px;
  font-weight: 700;
}
.container-header nav ul li a:hover {
  color: #fc00a8;
  transition: 1s;
}
@media (max-width: 750px) {
  .logo {
    margin: 0 auto;
  }
  .menu-desk {
    display: none;
  }
}
</style>

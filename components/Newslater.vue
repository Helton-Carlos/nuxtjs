<template>
  <section id="newslater">
    <div class="container-newslater">
      <form>
        <h3>Receba nossas novidades:</h3>
        <input type="text" name="texto" id="texto" placeholder="Digite seu e-mail" />
        <input type="submit" value="Enviar" />
      </form>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style>
.container-newslater {
  background-color: #0f195b;
  width: 80%;
  height: 190px;
  margin: 0 auto;
}

.container-newslater form {
  max-width: 70%;
  padding-top: 75px;
  text-align: center;
  display: flex;
  margin: 0 auto;
  align-items: center;
}

.container-newslater h3 {
  color: #fff;
  font-weight: 300;
}

.container-newslater input[type="text"] {
  padding: 10px 70px;
  margin: 0 auto;
}

.container-newslater input[type="submit"] {
  padding: 10px 50px;
  background-color: #fc00a8;
  border: none;
  color: #fff;
  font-size: 18px;
  box-shadow: 0 0 0.3em #fc00a8;
}

.container-newslater input[type="submit"]:hover {
  background-color: #756c6c;
  transition: 1s;
}

@media (max-width: 750px) {
  .container-newslater form {
    flex-direction: column;
    padding-top: 30px;
  }
  .container-newslater h3 {
    padding-bottom: 10px;
  }
  .container-newslater input[type="text"] {
    max-width: 100%;
    margin-bottom: 20px;
  }
}
</style>

<template>
  <section id="contato">
    <div class="container-contato">
      <div class="subtitulo">
        <img src="img/phone.png" alt="telefone" />
        <h2>CONTATO</h2>
      </div>

      <div class="mpas-container">
        <form action="">
          <input type="text" name="nome" id="nome" placeholder="Nome Completo" />
          <input type="email" name="email" id="email" placeholder="Digite seu e-mail" />
          <textarea
            name="formulario"
            placeholder="Digite seu texto"
            id="formulario"
            cols="30"
            rows="10"
          ></textarea>
          <input type="submit" value="Enviar" id="enviar" />
        </form>

        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3933.411399095815!2d-35.707896885208626!3d-9.645844593094461!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x70145b7c4226bdf%3A0xf03d8e7211702f12!2sR.%20Banc%C3%A1rio%20Jos%C3%A9%20Farias%20de%20Almeida%20-%20Jati%C3%BAca%2C%20Macei%C3%B3%20-%20AL!5e0!3m2!1spt-BR!2sbr!4v1611963099547!5m2!1spt-BR!2sbr"
          width="600"
          height="450"
          frameborder="0"
          style="border: 0"
          allowfullscreen=""
          aria-hidden="false"
          tabindex="0"
        ></iframe>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style>
.container-contato {
  max-width: 80%;
  margin: 50px auto;
}
.mpas-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.mpas-container form {
  display: flex;
  flex-direction: column;
  width: 40%;
}
.mpas-container input {
  padding: 15px 20px;
  margin-bottom: 20px;
  border-radius: 10px;
  border: 2px solid #756c6c;
}
.mpas-container input[type="submit"] {
  background-color: #fc00a8;
  font-size: 18px;
  color: #fff;
  border: 2px solid #fc00a8;
  box-shadow: 0 0 0.3em #fc00a8;
}
.mpas-container input[type="submit"]:hover {
  background-color: #850058;
  font-size: 18px;
  color: #fff;
  transition: 1s;
  border: 2px solid #850058;
}
.mpas-container textarea {
  padding: 15px;
  width: 100%;
  margin-bottom: 20px;
  border-radius: 10px;
  border: 2px solid #756c6c;
}

@media (max-width: 900px) {
  .mpas-container {
    flex-direction: column;
  }
  .mpas-container form {
    width: 100%;
  }
  .mpas-container iframe {
    width: 100%;
  }
}
</style>

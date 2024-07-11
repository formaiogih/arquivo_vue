<template>
  <!DOCTYPE html>

  <html lang="pt-br">
  
  <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <link rel="stylesheet" href="css/index.css" />
  
      <title>Página com Imagens</title>
  
  </head>
  
  <body>
  
      <header>
          <h1>IMPORTANTES FILÓSOFOS</h1>
          <h3><a href="#textovideo">E seus legados</a></h3>
      </header>
  <br>
  <main>
      <article>
          <img src="../assets/aristoteles.jpeg" alt="Imagem 1" width="800" height="700" id="aristoteles">
  
          <section class="imgtexto">
              <section id="responsivo">
                  <img src="../assets/platao.png" alt="Imagem 2" width="400" height="250" class="imgs">
  
                  <img src="../assets/socrates.jpg" alt="Imagem 3" width="400" height="250" class="imgs">
              </section>
              <br>
  
              <section class="p">
                  <p>Imagem 1: Aristóteles</p>
                  <p>Imagem 2: Platão</p>
                  <p>Imagem 3: Sócrates</p>
              </section>
              <hr>
              <hr>
          </section>
          <section id="textovideo">
              <section class="p" id="video">
                  <p>Conheça um pouco mais sobre o legado destes filósofos no vídeo ao lado!</p>
              </section>
            <iframe width="500" src="https://www.youtube.com/embed/QweIkJdyyYU?si=kWwP4iYHlBlErm57" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
          </section>
      </article>
  </main>
  <br>
      <footer>
          <p>Site feito por: Giovanna Formaio Reis</p>
          <p>Professor: Wagner Simões Santos</p>
          <p>Turma: IIW2022B</p>
      </footer>
  </body>
  
  </html>
</template>

<script>
export default {
name: 'HelloWorld',
};
</script>

<style scoped>
html{
  scroll-behavior:smooth;
}

article{
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  border-left: dotted 3px gray;
  border-right: dotted 3px gray;
  border-radius: 10px;
  padding: 10px;
  align-content: center;
  justify-content: center;
}

header{
  text-align: center;
  text-justify: center;
  background-color: rgb(179, 224, 255);
  height: fit-content;
  margin-top: -7px;
  border-radius: 10px;
  border: groove 2px rgb(98, 98, 190);
}

footer{
  text-align: center;
  text-justify: center;
  background-color: rgb(255, 222, 179);
  height: fit-content;
  margin-top: -7px;
  border-radius: 10px;
  border: groove 2px rgb(253, 179, 114);
  font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
  color: rgb(224, 86, 0);
}

h1, h3{
  font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
  color: rgb(44, 66, 85);
}

h1{
  margin-bottom: -10px;
}

.imgtexto {
  display: flex;
  flex-direction: column;
  align-content: space-around;
  align-content: space-between;
  margin: 20px;
  flex-wrap: wrap;
}

#responsivo {
  display: flex;
  flex-direction: column;
}

img {
  border-radius: 20px;
}

.p{
  background-color: rgb(255, 254, 188);
  border-radius: 10px;
  border: double 4px rgb(255, 123, 0);
  padding: 10px;
}

#textovideo{
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: center;
  height: 300px;
  width: 96%;
}

#video{
  margin-right: 10px;
  width: 47%;
  height: fit-content;
}

iframe{
  border-radius: 20px;
}

a{
  text-decoration: none;
  color: rgb(44, 66, 85);

}

@media (max-width: 1300px) {
  #responsivo {
      display: flex;
      flex-direction: row;
  }

  #video{
      width: 100%;
      margin-right: -10px;
      margin-bottom: 3%;
  }

  #textovideo{
      display: flex;
      flex-direction: column;
      align-items: center;
      width: 90%;
      margin-left: -1%;
      height: fit-content;
  }

  iframe{
      width: 102%;
      height: 400px;
  }
}

@media (max-width: 1010px) {
  #textovideo{
      display: flex;
      flex-direction: column;
      align-content: center;
  }
  
}

@media (max-width: 890px) {
  #responsivo {
      display: flex;
      flex-direction: column;
      align-content: center;
      justify-content: center;
  }

  #aristoteles{
      width: 90%;
  }

  .imgs{
      width: 95%;
      height: auto;
  }
  
}

@media (max-width: 500px){
  .imgs{
      width: 90%;
  }

  h1{
      font-size: 180%;
  }
}

</style>
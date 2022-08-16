<template>
    <section aria-label="Projetos" class="projetos" id="projetos">
      <div class="projetos-container">
        <h2 class="subtitulo">Projetos</h2>
        <div class="cards">
          <div class="card">
            <h3>CAKELICIOUS</h3>
            <a href="https://cakelicous.vercel.app">
              <img src="../assets/img/CakeliciousLogo.png" alt="Logo Cakelicious" width="301" height="130">
            </a>
            <div class="info-card">
              <p>Projeto feito durante o Workshop do Pet - UEM para uma loja de bolos</p>
              <a href="https://github.com/M4Barboza/Cakelicous">
                <img src="../assets/img/github.png" alt="Icone Github" width="22px" height="20px">
              </a>
            </div>
          </div>
          <div class="card">
            <h3>Cakelicious</h3>
            <a href="https://ignite-lab-silk.vercel.app/">
              <img src="../assets/img/ignite-lab.png" alt="Logo Ignite-Lab" width="301" height="130">
            </a>
            <div class="info-card">
              <p>Projeto feito durante o Ignite Lab da plataforma Rocketseat</p>
              <a href="https://github.com/M4Barboza/Ignite-Lab">
                <img src="../assets/img/github.png" alt="Icone Github" width="22px" height="20px">
              </a>
            </div>
          </div>
          <div class="card">
            <h3>Building👨‍💻</h3>
          </div>
        </div>
        
      </div>  
    </section>
</template>

<script>
export default {
  name: 'Projects',
}
</script>

<style>

.projetos{
  background-color: #00000088;

}

.projetos-container {
  max-width: 1200px;
  padding: 40px 20px;
  margin: 0 auto;
  display: grid;
  grid-template-columns: 1fr 2fr;
  gap: 100px;
}

.projetos-container .subtitulo {
  color: #141414;
}

.cards{
  margin: 0 auto;
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 25px;
}

.card{
  display: flex;
  flex-direction: column;
  max-width: 397px;
  height: 350px;
  align-items: center;
  justify-content: space-between;
  background-color: #00000081;
  border-radius: 4px;
  color: #fff;
  box-shadow:  10px 5px 0px rgba(0, 0, 0, 0.13);
}

.card a:hover{
  -moz-transform: scale(1.1);
	-webkit-transform: scale(1.1);
	transform: scale(1.1);
}

.card h3{
  margin: 40px 121px 22px;
  font-size: 1.125rem;
  line-height: 1.1;
  font-weight: bold;
}

.card a{
  margin-bottom: 20px;
}

.card .info-card{
  padding: 20px 20px;
  display: block;
  align-items: flex-start;
  color:#909090;
}

.card .info-card p{
  margin-bottom: 20px;
}

@media (max-width: 800px) {
  .projetos-container {
    grid-template-columns: 1fr;
    gap: 40px;
  }
  .projetos-container .subtitulo {
    color: #141414;
  }

  .cards{
    grid-template-columns: 1fr;
    gap: 40px;
  }
  .cards .card{
    max-width: 310px;
  }
}




</style>
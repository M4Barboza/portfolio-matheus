<template>
    <section aria-label="Experiência" class="experiencia" id="experiencia">
      <div class="experiencia-container">
        <h2 class="subtitulo">Experiência</h2>
        <div>
          <p class="experiencia-texto">Desenvolvo pequenos projetos e páginas estáticas com <strong>HTML</strong>,<strong>CSS</strong> e <strong>JavaScript</strong>. Além disso, estou aprendendo <strong>Vue.js</strong> e <strong>React</strong>.</p>  
          <div class="empresa">
                  <span class="empresa-ano">2022-2022</span>
                  <h3 class="empresa-titulo">Bitzen Tecnologia</h3>
                  <span class="empresa-titulo">Estagiário em Front End</span>
                  <p class="empresa-texto">Na Bitzen eu trabalhei com HTML, CSS, JavaScript e Vue.JS. Além disso, também trabalhei usando a metodologia de SCRUM.</p>
                  <ul class="empresa-habilidades">
                      <li>HTML</li>
                      <li>CSS</li>
                      <li>JavaScript</li>
                      <li>Git</li>
                      <li>Github</li>
                      <li>Gitflow</li>
                      <li>Vue.JS</li>
                  </ul>
          </div>
          <div class="empresa">
                  <span class="empresa-ano">2021-2022</span>
                  <h3 class="empresa-titulo">VG-Educacional</h3>
                  <span class="empresa-titulo">Estagiário em Front End</span>
                  <p class="empresa-texto">Na VG Educacional trabalhei pricipalmente com a ferramenta de criação de Webflow, semelhante ao Wordpress, realizava hot sites para eventos que a empresa participaria, também aprendi muito sobre JS e no fim estudei sobre Emails Marketing.</p>
                  <ul class="empresa-habilidades">
                      <li>HTML</li>
                      <li>CSS</li>
                      <li>JavaScript</li>
                      <li>Webflow</li>
                      <li>UX Design</li>
                      <li>UI Design</li>
                  </ul>
          </div>
          <div class="empresa">
                      <span class="empresa-ano">2021-2021</span>
                      <h3 class="empresa-titulo">CRMALL</h3>
                      <span class="empresa-titulo">Suporte Técnico</span>
                      <p class="empresa-texto">Como suporte técnico de nível N1 atendia os chamados de Shoppings para esclarecer dúvidas e dar suporte à aplicação que a empresa disponibilizava.</p>
          </div>
        </div>
      </div>
    </section>
</template>

<script>
export default {
    name: 'Experience',
}
</script>

<style>

.experiencia {
  background-color: #00000088;
}

.experiencia-container {
  max-width: 1200px;
  padding: 40px 20px;
  margin: 0 auto;
  display: grid;
  grid-template-columns: 1fr 2fr;
  gap: 100px;
  
}

.experiencia-container .subtitulo {
  color: #00F260;
}

.experiencia-texto {
  font-size: 1.5rem;
  line-height: 1.33;
  max-width: 40ch;
  margin-bottom: 60px;
  color: #141414;
}

.experiencia-texto strong {
  color: #141414;
}

.empresa {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 10px 20px;
  padding: 20px;
  position: relative;
  background: #00000081;
  margin-bottom: 20px;
  border-radius: 4px;
}

.empresa::before {
  content: "";
  display: block;
  width: 4px;
  height: 20px;
  background-image: linear-gradient(#0575E6, #00F260);
  position: absolute;
  top: 20px;
  left: -4px;
}

.empresa-ano {
  position: absolute;
  top: 22px;
  left: -100px;
  color: #000000;
  text-align: right;
  width: 80px;
  font-size: 0.875rem;
}

.empresa-titulo {
  font-size: 1.125rem;
  line-height: 1.1;
  font-weight: bold;
  color: #fff;
}

.empresa-texto {
  font-size: 0.875rem;
  line-height: 1.4;
  color: #909090;
}

.empresa-habilidades {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  align-content: start;
}

.empresa-habilidades li {
  font-size: 0.875rem;
  line-height: 1.4;
  border-radius: 4px;
  background: #909090;
  padding: 5px 10px;
}

.empresa-habilidades li:hover{
  background: #0575E6;
  color: #fff;
  cursor: default;
}

@media (max-width: 800px) {
  .experiencia-container {
    grid-template-columns: 1fr;
    gap: 40px;
  }
  .experiencia-container .subtitulo {
    color: #141414;
  }
  .experiencia-texto {
    font-size: 1.25rem;
  }
  .empresa-ano {
    position: initial;
    order: 1;
    width: initial;
    text-align: left;
  }
}

@media (max-width: 400px) {
  .empresa {
    grid-template-columns: 1fr;
  }
}

</style>
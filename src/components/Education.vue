<template>
    <section class="formacao" id="formacao" aria-label="formacao">
        <div class="formacao-container">
        <h2 class="subtitulo">Formação</h2>
        <div>
            <p class="formacao-texto">
            No momento estou me graduando em <strong>Bacharel em Informática </strong>pela <strong>UEM</strong>. Além disso me mantenho sempre atualizado com cursos intensivos online.
            </p>
            <div class="formacao-extra">
                <div class="cursos">
                    <h3>Cursos Intensivos</h3>
                    <ul>
                        <li>TI Academy<span>FullStack - React & Node.js</span></li>
                        <li>Cursos Origamid<span>Frontend/Design Web no geral</span></li>
                    </ul>
                </div>
                <div class="idiomas">
                    <h3>Idiomas</h3>
                    <ul>
                        <li>Inglês <span>Intermediário</span></li>
                        <li>Português <span>Nativo</span></li>
                    </ul>
                </div>
            </div>
        </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Education',
}
</script>

<style>

.formacao {
  background: #141414c0;
  color: #fff;
}

.formacao-container {
  max-width: 1200px;
  padding: 120px 20px;
  margin: 0 auto;
  display: grid;
  grid-template-columns: 1fr 2fr;
  gap: 100px;
  position: relative;
}

.formacao-container::after {
  content: "";
  display: block;
  width: 130px;
  height: 100px;
  background: url("../img/detalhe.svg") no-repeat center;
  position: absolute;
  bottom: -50px;
  left: 20px;
}

.formacao .subtitulo {
  color: #0575E6;
  max-width: 5ch;
}

.formacao-texto {
  font-size: 1.5rem;
  line-height: 1.33;
  max-width: 40ch;
  margin-bottom: 60px;
  color: #a3a3a3;
}

.formacao-texto strong {
  color: #fff;
}

.cursos {
  margin-bottom: 60px;
}

.formacao-extra h3 {
  font-size: 0.875rem;
  line-height: 1.4;
  color: #8f8f8f;
  text-transform: uppercase;
  margin-bottom: 30px;
  position: relative;
}

.formacao-extra h3::before {
  display: block;
  content: "";
  width: 24px;
  height: 24px;
  background: url("../assets/img/cursos.svg") no-repeat center center;
  position: absolute;
  left: -36px;
  top: -4px;
}

.cursos h3::before {
  background: url("../assets/img/cursos.svg") no-repeat center center;
}

.idiomas h3::before {
  background: url("../assets/img/idiomas.svg") no-repeat center center;
}

.formacao-extra li {
  font-size: 1.125rem;
  line-height: 1.1;
  margin-bottom: 20px;
}

.formacao-extra span {
  color: #8f8f8f;
}

.cursos li {
  display: flex;
  justify-content: space-between;
}

@media (max-width: 800px) {
  .formacao-container {
    grid-template-columns: 1fr;
    padding: 60px 20px;
    gap: 40px;
  }
  .formacao .subtitulo {
    color: #fff;
  }
  .formacao-texto {
    font-size: 1.25rem;
  }
  .formacao-extra h3::before {
    position: initial;
    margin-bottom: 10px;
  }
}

</style>
<template>
  <main class="introduction">
      <img src="../assets/img/perfil.svg" alt="Lobo Cinza" width="360" height="520">
    <Transition name="slide" appear="">
      <div>
        <h1>Desenvolvedor<br>Front End</h1>
        <p>Localizado em <span class="cidade">Maringá - PR</span> 🦊</p>
      </div>
    </Transition>
  </main>
</template>

<script>
export default {
    name: 'Introduction',
}
</script>

<style scoped>
.introduction {
  max-width: 1200px;
  padding: 40px 20px;
  margin: 0 auto;
  display: grid;
  grid-template-columns: 1fr 2fr;
  gap: 100px;
  align-items: center;
}

.introduction h1 {
  font-size: 4.5rem;
  line-height: 1.125;
  margin-bottom: 30px;
  position: relative;
}

.introduction h1::before {
  content: "";
  display: block;
  width: 130px;
  height: 100px;
  background: url(../assets/img/detalhe.svg) no-repeat center;
  position: absolute;
  top: -15px;
  left: -40px;
  z-index: -1;
}

.introduction p {
  font-size: 1.5rem;
  color: #525252;
}
.cidade{
  color: #0575E6;
}

@media (max-width: 1000px) {
  .introduction h1 {
    font-size: 3rem;
  }
}

@media (max-width: 800px) {
  .introduction {
    grid-template-columns: 1fr 1fr;
    gap: 40px;
  }
  .introduction h1 {
    font-size: 2rem;
  }
  .introduction h1::before {
    width: 30px;
    height: 10px;
    left: 0px;
  }
}

@media (max-width: 400px) {
  .introduction {
    grid-template-columns: 1fr;
  }
  .introduction img {
    display: none;
  }
}

.slide-enter-from{
  transform: translateX(-150px);
}

.slide-enter-active{
  transition:  2s;
}

.slide-enter-to{
  transform: translateX(0px);
}
</style>
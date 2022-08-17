<template>
  <header id="home" class="header">
    <img src="../assets/img/MatheusBarboza.png" alt="Lobo"  width="120" height="70">
    <nav>
      <ul class="header-menu">
        <li><a href="#experiencia" @click.prevent="scrollTo('#experiencia')">Experiência</a></li>
        <li><a href="#projetos" @click.prevent="scrollTo('#projetos')">Projetos</a></li>
        <li><a href="#formacao" @click.prevent="scrollTo('#formacao')">Formação</a></li>
        <li><a href="#contato" @click.prevent="scrollTo('#contato')">Contato</a></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'Header',
  methods:{
    scrollTo(selector){
      document.querySelector(selector).scrollIntoView({behavior: 'smooth'})
    }
  }
}
</script>

<style>

.header {
  height: auto;
  padding: 40px 20px;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.header-menu {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  justify-content: center;
}

.header-menu a {
  font-size: 1.125rem;
  line-height: 1.3;
  padding: 10px 20px;
  text-decoration: none;
  color: #141414;
}



@media (min-width: 800px){
  .header-menu a:hover{
    position:relative;
    width: 150px;
    height: 150px;
    border: solid #0575E6 2px;
    border-radius: 60% 40% 40% 20%;
  }
}

@media (max-width: 800px) {
  .header {
    flex-direction: column;
    gap: 40px;
    padding: 20px;
  }
    
  .header-menu{
    display: flex;
    flex-direction: column;
    align-items: center;
  }
    
  .header a {
    background: #000000;
    border-radius: 5px;
    font-size: 1rem;
    color: #fff;
    display: flex;
    justify-content: center;
    width: 75px;
  }
}

</style>
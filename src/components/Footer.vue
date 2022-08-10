<template>
  <footer class="footer" id="contato">
    <div class="footer-container">
      <p class="footer-texto">
        Estou em busca de estágios ou CLT de nível Júnior, entre em contato! 🦜
      </p>
      <ul class="footer-contato">
        <li>matheus.barboza0@gmail.com</li>
        <li>+55 (44) 99711-9193</li>
        <li><a href="https://github.com/M4Barboza">GitHub</a>🐙</li>
      </ul>
      <p class="footer-copy">Feito com 💚 por Matheus</p>
    </div>
  </footer>
</template>

<script>
export default {
    name: 'Footer',
}
</script>

<style>

.footer {
  background: #00000088;
}

.footer-container {
  padding: 120px 20px 60px 20px;
  margin: 0 auto;
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 100px;
  align-items: center;
}

.footer-texto {
  font-size: 1.5rem;
  line-height: 1.33;
  color: #cccccc;
}

.footer-container li {
  font-weight: bold;
  font-size: 2.25rem;
  line-height: 1.1;
  color: #ffffff;
  margin-bottom: 30px;
}

.footer-contato li a {
  color: #ffffff;
}

.footer-copy {
  grid-column: 1 / -1;
  font-size: 1.125rem;
  color: #8f8f8f;
}

@media (max-width: 800px) {
  .footer-container {
    grid-template-columns: 1fr;
    gap: 40px;
  }
  .footer-container li {
    font-size: 1.2rem;
  }
}

</style>
<template>
  <footer class="footer">
    <p>Developed with ❤️ by <a href="https://andresparra.vercel.app">Andrés Parra Garzón</a></p>
  </footer>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style scoped>
  .footer {
    text-align: center;
    position: absolute;
    bottom: 20px;
    left: 50%;
    transform: translateX(-50%);
    color: #fff;
    text-shadow: 2px 2px 5px #111;
    font-weight: bold;
  }
  .footer a {
    color: tomato;
  }
</style>
<template lang="html">
  <div class="header">
    <a @click="scroll" class="text-decoration-none pizza-header">
      <h1 class="text-center display-2 text-uppercase pizza-h1">Pizza</h1>
      <h2 class="text-center display-4 text-dark pizza-h2">piz·za</h2>
      <h3 class="text-center display-5 text-secondary">/ˈpētsə/</h3>
    </a>
  </div>
</template>

<script>
export default {
  name: 'Header',

  methods: {
      scroll: function() {
        const element = document.getElementById('nav');
        element.scrollIntoView({ behavior: 'smooth' });
      }
    }
}


</script>

<style lang="css" scoped>
.header {
  /* padding: 5rem 0 6rem; */
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background-color: #FEFAEE;
}

h1 {
  color: #FA5D29;
}

.pizza-h2 {
  padding-bottom: 1.25rem;
}

.pizza-header {
  cursor: pointer;
}
</style>

<script setup>
  import AsideCi from './components/Aside.vue'
  import HeaderCi from './components/Header.vue'
  import SectionCi from './components/Section.vue'
</script>


<template>
  <body>
    <div class="carnet">
      <AsideCi/>
      <main>
        <header><HeaderCi/></header>
        <section><SectionCi/></section>         
      </main>
    </div>
  </body>
</template>


<style scoped>
  *{
    border: 0;
    margin: 0;
    padding: 0;
  }

  body{
    display: flex;
    justify-content: center;
    align-items: center;
    height: 60vh;
    font-size: 10px;
    font-family: sans-serif;
    margin-top: -290px;
  }

  .carnet{
    width: 400px;
    height: 230px;
    background: #c8deed;
    border-radius: 20px;
    display: grid;
    grid-template-columns: 30% 1fr;
    padding: 15px;
    box-shadow: 0px 0px 10px 2px black;
  }

  main{
    padding: 0px 14px;
  }
</style>
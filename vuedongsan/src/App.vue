<template>
  <div class="menu">
    <a v-for="name in menus" :key="name">{{ name }}</a>
  </div>

  <div v-for="(prodoct, i) in prodocts" :key="(prodoct, i)">
    <h4>{{ prodoct }}</h4>
    <p>{{ prize[i] }}</p>
  </div>
</template>

<script>

export default {
  name: 'App',
  data(){
    return {
      menus: ['Home','Shop','About'],
      prodocts: ['역삼동원룸', '천호동원룸', '마포구원룸'],
      prize: ['80 만원', '90 만원', '70 만원']
    }
  },
  components: {
  
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.menu{
  background-color: #005ab5;
  padding: 15px;
  border-radius: 5px;
}

.menu a{
  color: azure;
  padding: 10px;
}
</style>

<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <h1>{{ Num }}</h1>
    <HelloWorld 
      msg="Welcome to Your Vue.js App"
      @click_component="handleChangeNum()"
    />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld
  },
  state : {
    Num : 0
  },

  methods: {
      handleChangeNum() {
        console.log("lyx" , "click_component at App.vue");
        Num++;
      }
    //
  }
}
</script>

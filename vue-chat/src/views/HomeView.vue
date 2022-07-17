<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <!-- <chatApp/> -->
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
// import chatApp from '@/components/chatApp.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld
    // chatApp,
  }
}
</script>

<template lang="pug">
  .home
    img(alt='Vue logo', src='../assets/logo.png')
    b-alert(show) Default Alert
    hello-world(msg='Welcome to Your Vue.js App')
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "home",
  components: {
    HelloWorld
  }
};
</script>

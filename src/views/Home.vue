<template>
  <div class="home">
    <router-link to="/about">跳转</router-link>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "Home",
  data() {
    return {
      show: false
    };
  },
  components: {
    HelloWorld
  }
};
</script>
<style scoped>
.home {
  height: 100%;
  background: yellow;
}

</style>

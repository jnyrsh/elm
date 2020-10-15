<template>
  <div id="app">
    
    <transition name="left">

    <router-view class="router" />
    </transition>
  </div>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
html,body,#app{
  height: 100%;
}
#add>div{
  height: 100%;
}
*{
  margin: 0;
}
.left-enter{
  transform: translateX(100%)
}
.left-enter-to{
  transform: translateX(0)
}
.left-enter-active,.left-leave-active{
  transition: all 2s;
}
.left-leave{
  transform: translateX(0);
}
.left-leave-to{
     transform: translateX(-100%)
}
.router{
  position: absolute;
  width: 100%;
}
</style>

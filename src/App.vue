<template>
  <div id="app" class="bg-gray-700">
    <main-view />
  </div>
</template>

<script>
import MainView from "./components/MainView.vue";

export default {
  name: 'app',
  components: { MainView },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style lang="sass">
@import './assets/sass/index.sass'
</style>

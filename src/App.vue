<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'

export default {
  name: 'ViteComics',
  components: {
    AppHeader, AppMain
  }
};
</script>


<template>
  <AppHeader />
  <AppMain />
</template>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

.container {
  width: 1200px;
  margin: 0 auto;
}
</style>
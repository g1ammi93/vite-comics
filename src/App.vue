<script>
import AppHeader from './components/AppHeader.vue'

export default {
  name: 'ViteComics',
  components: {
    AppHeader
  }
};
</script>


<template>
  <AppHeader />
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
<template>
  <TopBar />
  <div class="main-container container d-flex flex-row">
      <div class="container m-0 p-0 main-info">
          <RouterView />
      </div>
  </div>
</template>
<script>
import TopBar from './components/topbar/TopBar.vue';
export default {
  components: {
      TopBar,
  },
  
  
}
</script>
<style>
  .main-info {
    width: 100%;
  }
  
  .main-container {
    margin-top: 30px
  }
</style>
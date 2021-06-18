<template>
  <div class="home flex-grow-1 d-flex flex-column align-items-center justify-content-center">
    <img src="https://ih1.redbubble.net/image.1483730416.8031/tst,small,507x507-pad,600x600,f8f8f8.jpg" alt="CodeWorks Logo">
    <h1 class="my-5 bg-dark text-light p-3 rounded d-flex align-items-center">
      <span class="mx-2 text-white">OSRS</span>
    </h1>
  </div>
  <div id="app">
    {{ info }}
  </div>
</template>

<script>
export default {
  name: 'Home',
  setup() {
    return {
      account: computed(() => AppState.account)
    }
  }
}
</script>

<style scoped lang="scss">
.home{
  text-align: center;
  user-select: none;
  > img{
    height: 200px;
    width: 200px;
  }
}
</style>

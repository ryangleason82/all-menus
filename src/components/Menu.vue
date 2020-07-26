<template>
  <div class="container">
    <InputMenu />
    <OutputMenu />
  </div>

  
</template>

<script>
import OutputMenu from './OutputMenu'
import InputMenu from './InputMenu'
export default {
  name: 'Menu',
  components: {
    OutputMenu,
    InputMenu
  }
}
</script>

<style scoped>
</style>

<template>
  <div>
    <h1 class="mt-4 text-center">Menu</h1>
    <div v-for="menu in menuData" :key="menu.title">
      <h4 class="mt-4 text-left">{{ menu.category }}</h4>
      <hr />
      <div v-for="item in menu.items" :key="item.title">
        <h5 class="mt-4">{{ item.title }}</h5>
        <p>{{ item.description }}</p>
      </div>
    </div>
  </div>
</template>

<script>
const menuList = require("../data/Menu.json");
export default {
  name: "OutputMenu",
  data() {
    return {
      menuData: [],
    };
  },
  mounted() {
    this.menuData = menuList;
  },
};
</script>

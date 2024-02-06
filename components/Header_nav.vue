<template>
  <div class="header">
  <h1><img src="~/assets/images/logo.png" width="200px" ></h1>
<span @click="isOpen = !isOpen">
      <span v-if="!isOpen"><Icon name="game-icons:hamburger-menu" color="white" style="font-size:2rem" /></span>
      <span v-else><Icon name="material-symbols:close-rounded" color="white" style="font-size:2rem" /></span>
    </span>


    </div>
        <div v-if="isOpen">
      <ul class="menu-items">
        <li v-for ="item in menuItems" :key="item">{{ item }}</li>
      </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isOpen: false,
      menuItems: ['Menu Item 1', 'Menu Item 2', 'Menu Item 3']
    };
  },
};
</script>

<style>
.menu-items{
  background-color:#333;
  position:absolute;
  top:0;
  right:0;
  height:100%;
  transition:  all 1s linear;   /*１秒掛けて開く。速度は一定*/
}
</style>
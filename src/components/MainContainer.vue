<template>
  <div class="page-container">
    <md-app md-waterfall md-mode="overlap">
      <TopAppBar :menu-visible="menuVisible"/>

      <Drawer :menu-visible="menuVisible"/>

      <Content/>
    </md-app>
  </div>
</template>

<style scoped>
  .md-app {
    max-height: 400px;
    border: 1px solid rgba(0,0,0, .12);
  }

   
  .md-drawer {
    width: 230px;
    max-width: calc(100vw - 125px);
  }
</style>

<script>
import Drawer from "./Drawer";
import TopAppBar from "./TopAppBar";
import Content from "./Content";

export default {
  name: 'Overlap',
  components: {Content, TopAppBar, Drawer},
  data: () => ({
    menuVisible: false
  })
}
</script>

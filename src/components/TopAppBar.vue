<template>
  <md-app-toolbar class="md-primary md-large">
    <div class="md-toolbar-row">
      <md-button class="md-icon-button" @click="menuVisible = !menuVisible">
        <md-icon>menu</md-icon>
      </md-button>

      <span class="md-title">My Title</span>
    </div>
  </md-app-toolbar>
</template>
<script>
export default {
  name: 'TopAppBar',
  props: {
    menuVisible: {}
  }
}
</script>

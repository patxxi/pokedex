<template>
  <div id="layout">
    <HeaderComponent></HeaderComponent>
    <slot name="content"></slot>

    <FooterComponent></FooterComponent>
  </div>
</template>

<script>
export default {
  name: "LayoutComponent",
};
</script>
<script setup>
import HeaderComponent from "@components/Header/HeaderComponent.vue";
import FooterComponent from "@components/Footer/FooterComponent.vue";
</script>

<style scoped>
#layout {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 100%;
  min-height: 100vh;
}
</style>

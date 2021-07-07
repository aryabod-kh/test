<style lang="scss" scoped>
#app {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 100%;
}
</style>
<template>
  <section id="app">
    <Nuxt />
  </section>
</template>
<script lang="ts">
import { Vue, Component, Prop, Watch, Emit, Ref } from "vue-property-decorator";

@Component
export default class component_name extends Vue {}
</script>
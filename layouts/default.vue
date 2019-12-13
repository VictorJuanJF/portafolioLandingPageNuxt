<template>
  <div>
    <app-header></app-header>
    <main>
      <fade-transition origin="center" mode="out-in" :duration="250">
        <nuxt />
      </fade-transition>
    </main>
  </div>
</template>

<script>
import appHeader from "@/components/appHeader";
import { FadeTransition } from "vue2-transitions";
export default {
  components: {
    FadeTransition,
    appHeader
  }
};
</script>

<style lang="scss" scoped>
</style>

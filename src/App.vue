<script setup>
import PartNavBar from '@/components/PartNavBar.vue'
import Section01 from '@/components/Section01.vue'
import Section02 from '@/components/Section02.vue'
</script>

<template>
  <PartNavBar class="partnavbar"></PartNavBar>
  <Section01></Section01>
  <Section02></Section02>
</template>

<style scoped>
.partnavbar {
  position: fixed;
  z-index: 9999;
}

</style>

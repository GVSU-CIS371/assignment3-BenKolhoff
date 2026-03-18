<template>
  <div class="syrup" :style="{ backgroundColor: props.syrupColor, height: props.syrupColor === '#c6c6c6' ? '0%' : '20%' }"></div>
</template>

<script setup lang="ts">
type SyrupProp = {
  syrupColor: string;
};
const props = defineProps<SyrupProp>();
</script>
<style lang="scss" scoped>
.syrup {
  transform: translateY(400%);
  background-color: #c6c6c6;
  position: relative;
  width: 100%;
  height: 20%;
  animation: pour-tea 2s 1s forwards;
  z-index: 2;
}
</style>

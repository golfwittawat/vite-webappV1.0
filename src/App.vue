<template>
  <RouterView />
</template>

<script>
  // ประกาศตัวแปลชื่อเวป
  const brand = " | Smart Inventory"

export default {
  watch:{
    $route(to){
      document.title = to.meta.title + brand
    }
  }
};
</script>

<style scoped></style>

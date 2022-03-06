<script setup lang="ts">
import CartProduct from './CartProduct.vue';
const props = defineProps<{
  cart: ProductCartInterface[];
}>();
</script>

<template>
  <div class="d-flex flex-column">
    <CartProduct v-for="product of cart" :product="product" />
  </div>
</template>

<style lang="scss" scoped></style>

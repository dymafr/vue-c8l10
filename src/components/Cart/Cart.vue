<script setup lang="ts">
import CartProductList from './CartProductList.vue';

const props = defineProps<{
  cart: ProductCartInterface[];
}>();
</script>

<template>
  <div class="p-20">
    <h2 class="mb-10">Panier</h2>
    <CartProductList :cart="cart" />
  </div>
</template>

<style lang="scss" scoped></style>

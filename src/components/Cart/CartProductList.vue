<script setup lang="ts">
import CartProduct from './CartProduct.vue';
import type { ProductInterface } from '@/interfaces';

const props = defineProps<{
  cart: ProductInterface[];
}>();
</script>

<template>
  <div class="d-flex flex-column">
    <CartProduct v-for="product of cart" :product="product" />
  </div>
</template>

<style lang="scss" scoped></style>

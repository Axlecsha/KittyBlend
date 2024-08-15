<script setup>
import DrawerHead from './DrawerHead.vue'
import CartItemList from './CartItemList.vue'
</script>

<template>
  <div class="fixed top-0 left-0 h-full w-full bg-black z-10 opacity-65"></div>
  <div class="bg-white w-96 h-full fixed right-0 top-0 z-20 p-8">
    <DrawerHead />
    <CartItemList />
    <div class="flex flex-col gap-4 mt-7">
      <div class="flex gap-2">
        <span>Итого:</span>
        <div class="flex-1 border-b border-dashed"></div>
        <b>1505 ₽</b>
      </div>
      <div class="flex gap-2">
        <span>Доставка:</span>
        <div class="flex-1 border-b border-dashed"></div>
        <b>127 ₽</b>
      </div>
      <button
        disabled=""
        class="transition bg-lime-500 w-full disabled:bg-slate-300 rounded-xl py-3 text-white hover:bg-lime-600 active:bg-lime-700 cursor-pointer mt-4"
      >
        Оформить заказ
      </button>
    </div>
  </div>
</template>

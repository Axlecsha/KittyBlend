<script setup>
import Header from './components/Header.vue'
import CardList from './components/CardList.vue'
import Drawer from './components/Drawer.vue'
</script>

<template>
  <!--<Drawer /> -->
  <div class="bg-white w-4/5 m-auto rounded-xl shadow-xl mt-14">
    <Header />
    <div class="p-10">
      <div class="flex justify-between items-center">
        <h2 class="text-3xl font-bold mb-8">Все котята</h2>
        <div class="flex gap-4">
          <select class="py-2 px-3 border rounded-md outline-none my-2 pl-4 pr-2">
            <option>Сначала популярные</option>
            <option>Сначала недорогие</option>
            <option>Сначала дорогие</option>
          </select>
          <div class="relative">
            <img class="absolute left-4 top-5" src="/search.svg" />
            <input
              class="border rounded-md my-2 py-2 pl-11 pr-4 outline-none focus:border-gray-400 transition"
              placeholder="Поиск..."
            />
          </div>
        </div>
      </div>
      <CardList />
    </div>
  </div>
</template>

<style scoped></style>

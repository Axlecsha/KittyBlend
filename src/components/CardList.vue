<script setup>
import Card from './Card.vue'

const onClickAdd = () => {
  alert('Добавить!')
}
</script>

<template>
  <div class="grid grid-cols-4 gap-5">
    <Card
      title="Космический котёнок Марс"
      :price="1505"
      image-url="/cats/cat-1.jpg"
      :onClickAdd="onClickAdd"
    />
    <Card image-url="/cats/cat-2.jpg" />
    <Card image-url="/cats/cat-3.jpg" />
    <Card image-url="/cats/cat-4.jpg" />
    <Card image-url="/cats/cat-5.jpg" />
    <Card image-url="/cats/cat-6.jpg" />
    <Card image-url="/cats/cat-7.jpg" />
    <Card image-url="/cats/cat-8.jpg" />
    <Card image-url="/cats/cat-9.jpg" />
    <Card image-url="/cats/cat-10.jpg" />
    <Card image-url="/cats/cat-11.jpg" />
    <Card image-url="/cats/cat-12.jpg" />
  </div>
</template>

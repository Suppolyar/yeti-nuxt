<template>
  <section class="container mx-auto">
    <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-12 mb-6">
      <div
          v-for="card in cards"
          :key="card"
          class="">
        <NuxtLink
            to="/products"
            class="hover:shadow-2xl duration-300 p-3">
          <div class="mx-auto mb-3">
            <img class="w-full" src="~/assets/images/background.jpg" alt="product">
          </div>
          <div class="text-center text-2xl">{{ card.title }}</div>
        </NuxtLink>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "catalog",
  data() {
    return {
      cards: [
        {id: 1, title: 'World Eggs'},
        {id: 2, title: 'Мёд l Варенье'},
        {id: 3, title: 'Мясо'},
        {id: 4, title: 'Рыба'},
        {id: 5, title: 'Колбаса'},
        {id: 6, title: 'Сыр'},
        {id: 7, title: 'Йогурты'},
        {id: 8, title: 'Паста и равиоли'},
        {id: 9, title: 'Десерты'},
        {id: 10, title: 'Микрозелень'},

      ]
    }
  }
}
</script>

<style scoped>

</style>

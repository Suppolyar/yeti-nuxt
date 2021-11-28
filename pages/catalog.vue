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
          <div class="text-center text-base md:text-2xl">{{ card.title }}</div>
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

    }
  },
  computed: {
    cards() {
      return this.$store.state.cards
    }
  }
}
</script>

<style scoped>

</style>

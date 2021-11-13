<template>
  <section class="container mx-auto">
    <div class="grid grid-cols-5 sm:grid-cols-6">
      <div class="col-span-1 hidden sm:block">
        <div
            class="text-sm"
            v-for="card in cards"
            :key="card">
          <NuxtLink
              class="text-black text-opacity-100 hover:text-opacity-50 duration-300"
              to="/">{{ card.title }}
          </NuxtLink>
        </div>
      </div>

      <div class="col-span-5">
        <img class="w-full" src="~/assets/images/product-bg.jpg" alt="bg">
        <div class="grid grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-9 mb-6">
          <div
              v-for="item in items"
              :key="item"
              class="hover:shadow-2xl duration-300 p-3">
            <NuxtLink
                to="/"
                class="hover:shadow-2xl duration-300 p-3">
              <div class="mx-auto mb-3">
                <img class="w-full" src="~/assets/images/product-item.jpg" alt="product">
              </div>
              <div class="text-base font-bold">{{ item.title }}</div>
              <div class="text-xs">{{ item.description }}</div>
              <div class="text-sm font-bold">{{ item.price }}</div>
            </NuxtLink>
          </div>
        </div>
        <div class="text-center">
          <v-pagination
              :length="15"
              :total-visible="7"
          ></v-pagination>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "",
  data() {
    return {


    }
  },
  computed: {
    items() {
      return this.$store.state.items
    },
    cards() {
      return this.$store.state.cards
    }
  }
}
</script>

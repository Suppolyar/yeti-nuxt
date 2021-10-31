<template>
  <section class="container mx-auto">
    <div class="grid grid-cols-2 mb-12">
      <!--      Немного непонятно реализация в макете того, чего тут-->
      <!--      должно быть, но я вижу тут слайдер на подобии https://codesandbox.io/s/j6yks -->
      <!--      вот этого.-->
      <div class="sm:ml-auto md:pl-20 pt-6">
        <img src="~/assets/images/product-item-2.png" alt="product">
      </div>
      <div class="pl-6 pt-6">
        <div class="mb-6 text-xl md:text-2xl font-bold">Spicy ginger preserve</div>
        <div class="mb-6 text-base md:text-xl">Описание Spicy ginger preserve
          150 мл
        </div>
        <div class="mb-6 text-xl md:text-2xl font-bold">₽ 450</div>
        <div class="mb-6 flex flex-row">
          <v-btn
              class="mx-2"
              fab
              dark
              small
              color="primary"
          >
            <v-icon dark>
              mdi-minus
            </v-icon>
          </v-btn>
          <v-btn
              class="mx-2"
              fab
              dark
              small
              color="primary"
          >
            2
          </v-btn>
          <v-btn
              class="mx-2"
              fab
              dark
              small
              color="primary"
          >
            <v-icon dark>
              mdi-plus
            </v-icon>
          </v-btn>
        </div>
        <div class="hidden md:block">
          <v-btn
              large
              dark
              color="primary"
          >
            Добавить в корзину
          </v-btn>
        </div>
        <div class="block md:hidden">
          <v-btn
              small
              dark
              color="primary"
          >
            Добавить в корзину
          </v-btn>
        </div>
      </div>
    </div>
    <div class="text-center text-2xl mb-6">
      Вместе с этим товаром покупают
    </div>
    <div class="flex flex-row flex-wrap md:flex-nowrap justify-center md:justify-between">
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
  </section>
</template>

<script>


export default {
  name: "productItem",
  data() {
    return {
      items: [
        {id: 1, title: 'Spicy ginger Preserve YETI', description: 'Имбирное варенье описание товара', price: '₽ 650'},
        {id: 2, title: 'Spicy ginger Preserve YETI', description: 'Имбирное варенье описание товара', price: '₽ 650'},
        {id: 3, title: 'Spicy ginger Preserve YETI', description: 'Имбирное варенье описание товара', price: '₽ 650'},
        {id: 4, title: 'Spicy ginger Preserve YETI', description: 'Имбирное варенье описание товара', price: '₽ 650'}
      ]
    }
  },
}
</script>

<style scoped>

</style>

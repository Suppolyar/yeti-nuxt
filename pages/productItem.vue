<template>
  <section class="container mx-auto">
    <div class="grid grid-cols-2 mb-12">
      <div class="sm:ml-auto md:pl-20 pt-6">
        <div class="mb-3">
          <img class="w-2/3 mx-auto" src="~/assets/images/product-item-2.png" alt="product">
        </div>
        <div class="grid grid-cols-2 gap-x-3">
          <img src="~/assets/images/product-item-3.png" alt="product">
          <img src="~/assets/images/product-item-4.png" alt="product">
        </div>
      </div>
      <div class="pl-6 pt-6">
        <div class="mb-6 text-xl md:text-2xl font-bold">Spicy ginger preserve</div>
        <div class="mb-6 text-base md:text-xl">Описание Spicy ginger preserve
          150 мл
        </div>
        <div class="mb-6 text-xl md:text-2xl font-bold">₽ 450</div>
        <div class="mb-6 flex flex-row">
          <button class="bg-white transition duration-300 hover:bg-gray-100 text-gray-800 py-2 px-4 border border-solid border-black mr-1">
            -
          </button>
          <button class="bg-white transition duration-300 hover:bg-gray-100 text-gray-800 py-2 px-4 border border-solid border-black mr-1">
            2
          </button>
          <button class="bg-white transition duration-300 hover:bg-gray-100 text-gray-800 py-2 px-4 border border-solid border-black mr-1">
            +
          </button>
        </div>
        <div class="block">
          <button class="bg-black transition duration-300 hover:bg-opacity-80 text-white py-2 px-4 border border-solid border-black mr-1">
            Добавить в корзину
          </button>
        </div>
      </div>
    </div>
    <div class="text-center text-2xl mb-6">
      Вместе с этим товаром покупают
    </div>
    <div class="flex flex-row flex-wrap md:flex-nowrap justify-center md:justify-between">
      <div class="hover:shadow-2xl duration-300 p-3">
        <NuxtLink
            to="/"
            class="hover:shadow-2xl duration-300 p-3">
          <div class="mx-auto mb-3">
            <img class="w-full" src="~/assets/images/product-item.jpg" alt="product">
          </div>
          <div class="text-base font-bold">Spicy ginger Preserve YETI</div>
          <div class="text-xs">Имбирное варенье описание товара</div>
          <div class="text-sm font-bold">₽ 650</div>
        </NuxtLink>
      </div>
      <div class="hover:shadow-2xl duration-300 p-3">
        <NuxtLink
            to="/"
            class="hover:shadow-2xl duration-300 p-3">
          <div class="mx-auto mb-3">
            <img class="w-full" src="~/assets/images/product-item.jpg" alt="product">
          </div>
          <div class="text-base font-bold">Spicy ginger Preserve YETI</div>
          <div class="text-xs">Имбирное варенье описание товара</div>
          <div class="text-sm font-bold">₽ 650</div>
        </NuxtLink>
      </div>
      <div class="hover:shadow-2xl duration-300 p-3">
        <NuxtLink
            to="/"
            class="hover:shadow-2xl duration-300 p-3">
          <div class="mx-auto mb-3">
            <img class="w-full" src="~/assets/images/product-item.jpg" alt="product">
          </div>
          <div class="text-base font-bold">Spicy ginger Preserve YETI</div>
          <div class="text-xs">Имбирное варенье описание товара</div>
          <div class="text-sm font-bold">₽ 650</div>
        </NuxtLink>
      </div>
      <div class="hover:shadow-2xl duration-300 p-3">
        <NuxtLink
            to="/"
            class="hover:shadow-2xl duration-300 p-3">
          <div class="mx-auto mb-3">
            <img class="w-full" src="~/assets/images/product-item.jpg" alt="product">
          </div>
          <div class="text-base font-bold">Spicy ginger Preserve YETI</div>
          <div class="text-xs">Имбирное варенье описание товара</div>
          <div class="text-sm font-bold">₽ 650</div>
        </NuxtLink>
      </div>
    </div>
  </section>
</template>

<script>


export default {
  name: "productItem",
  data() {
    return {}
  },
  computed: {
    items() {
      return this.$store.state.items
    }
  }
}
</script>

<style scoped>

</style>

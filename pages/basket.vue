<template>
  <section class="container mx-auto">
    <div>
      <div class="text-black text-5xl text-center mb-6">Корзина</div>
      <div>
        <ul class="hidden xl:grid grid-cols-6 text-center mb-3">
          <li>Артикул</li>
          <li>Фото</li>
          <li>Описание</li>
          <li>Количество</li>
          <li>Цена</li>
          <li>Действие</li>
        </ul>
        <div class="grid grid-cols-3 xl:grid-cols-6 items-center text-center mb-6 p-3 xl:p-6 border border-black">
          <div>
            #145634
          </div>
          <div>
            <img class="mx-auto" src="~/assets/images/item-basket.png" alt="basket-item">
          </div>
          <div class="text-left">
            <p class="text-xl font-bold">Spicy ginger preserve</p>
            <p>Описание Spicy ginger preserve</p>
            <p>150 мл</p>
          </div>
          <div>
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
          <div>
            <p>450 ₽ </p>
          </div>
          <div>
            <button class="bg-white transition duration-300 hover:bg-gray-100 text-gray-800 py-2 px-4 border border-solid border-black mr-1">
              &#10005;
            </button>
          </div>
        </div>
        <div class="text-right mb-3">
          <p>Общая сумма: <span class="font-bold">2650 ₽</span></p>
        </div>
        <div class="flex flex-row justify-end items-center">
          <nuxt-link to="products"><span
              class="border-b opacity-70 hover:opacity-100 border-black transition duration-300">Продолжить покупки</span>
          </nuxt-link>
          <button class="bg-black transition duration-300 hover:bg-opacity-80 text-white py-2 px-4 border border-solid border-black ml-3">
            Добавить в корзину
          </button>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "basket"
}
</script>

<style scoped>

</style>

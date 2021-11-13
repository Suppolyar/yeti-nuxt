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
              1
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
          <div>
            <p>450 ₽ </p>
          </div>
          <div>
            <v-btn
                class="mx-2"
                fab
                dark
                small
                color="primary"
            >
              <v-icon dark>
                mdi-close
              </v-icon>
            </v-btn>
          </div>
        </div>
        <div class="text-right mb-3">
          <p>Общая сумма: <span class="font-bold">2650 ₽</span></p>
        </div>
        <div class="flex flex-row justify-end items-center">
          <nuxt-link to="products"><span
              class="border-b opacity-70 hover:opacity-100 border-black transition duration-300">Продолжить покупки</span>
          </nuxt-link>
          <v-btn
              class="ml-6"
              large
              dark
              color="primary"
          >
            Оформить заказ
          </v-btn>
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

<template>
  <section class="container mx-auto">
    <div class="text-black text-5xl text-center mb-6">Личный кабинет</div>
    <div class="text-2xl mb-6">Здравствуйте, Анна! Добро пожаловать в Ваш личный кабинет</div>
    <div class="xl:grid grid-cols-2 gap-x-6">
      <v-form v-model="valid">
        <div>Личные данные:</div>
        <div class="grid grid-cols-2 gap-x-6">
          <div>
            <label class=" tracking-wide text-gray-700 text-xs  mb-2" for="name">
              Имя
            </label>
            <input class="appearance-none block w-full bg-white text-gray-700 border border-black py-3 px-4 leading-tight focus:outline-none focus:bg-grey-100 focus:border-gray-500 border-solid" id="name" type="text" placeholder="Анна">
          </div>
          <div>
            <label class=" tracking-wide text-gray-700 text-xs  mb-2" for="last-name">
              Фамилия
            </label>
            <input class="appearance-none block w-full bg-white text-gray-700 border border-black py-3 px-4 leading-tight focus:outline-none focus:bg-grey-100 focus:border-gray-500 border-solid" id="last-name" type="text" placeholder="Петрова">
          </div>
          <div>
            <label class=" tracking-wide text-gray-700 text-xs  mb-2" for="email-address">
              Е-mail-адрес
            </label>
            <input class="appearance-none block w-full bg-white text-gray-700 border border-black py-3 px-4 leading-tight focus:outline-none focus:bg-grey-100 focus:border-gray-500 border-solid" id="email-address" type="email" placeholder="email@mail.ru">
          </div>
          <div>
            <label class=" tracking-wide text-gray-700 text-xs  mb-2" for="phone-number">
              Телефон
            </label>
            <input class="appearance-none block w-full bg-white text-gray-700 border border-black py-3 px-4 leading-tight focus:outline-none focus:bg-grey-100 focus:border-gray-500 border-solid" id="phone-number" type="number" placeholder="+7 911 250 38 68">
          </div>
        </div>
        <div>
          <label class=" tracking-wide text-gray-700 text-xs  mb-2" for="country">
            Страна
          </label>
          <div class="relative">
            <select class="appearance-none block w-full bg-white text-gray-700 border border-black py-3 px-4 leading-tight focus:outline-none focus:bg-grey-100 focus:border-gray-500 border-solid" id="country">
              <option>Россия</option>
              <option>Казахстан</option>
              <option>Беларусь</option>
            </select>
            <div class="pointer-events-none absolute inset-y-0 right-0 flex items-center px-2 text-gray-700">
              <svg class="fill-current h-4 w-4" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z"/></svg>
            </div>
          </div>
        </div>
        <div>
          <div>
            <label class=" tracking-wide text-gray-700 text-xs  mb-2" for="city">
              Населенный пункт
            </label>
            <input class="appearance-none block w-full bg-white text-gray-700 border border-black py-3 px-4 leading-tight focus:outline-none focus:bg-grey-100 focus:border-gray-500 border-solid" id="city" type="text" placeholder="Москва">
          </div>
        </div>
        <div class="grid grid-cols-2 gap-x-6">
          <div>
            <label class=" tracking-wide text-gray-700 text-xs  mb-2" for="region">
              Область
            </label>
            <input class="appearance-none block w-full bg-white text-gray-700 border border-black py-3 px-4 leading-tight focus:outline-none focus:bg-grey-100 focus:border-gray-500 border-solid" id="region" type="text" placeholder="Московская">
          </div>
          <div>
            <label class=" tracking-wide text-gray-700 text-xs  mb-2" for="post-id">
              Почтовый индекс
            </label>
            <input class="appearance-none block w-full bg-white text-gray-700 border border-black py-3 px-4 leading-tight focus:outline-none focus:bg-grey-100 focus:border-gray-500 border-solid" id="grid-last-name" type="post-id" placeholder="004156">
          </div>
        </div>
      </v-form>
      <div>
        <div class="mb-6">Заказы</div>
        <div class="flex flex-row justify-between items-center border border-black p-6 mb-6">
          <button class="bg-white transition duration-300 hover:bg-gray-100 text-gray-800 py-2 px-4 border border-solid border-black mr-1">
            &#10005;
          </button>
          <div class="text-left">
            <p class="font-bold">№ 74687474 от 28.06.2021</p>
            <p>Оплачен. Заказ выполнен</p>
          </div>
          <div>
            1450 ₽
          </div>
          <img src="~/assets/images/icons/union.svg" alt="union">
        </div>
        <div class="flex flex-row justify-between items-center border border-black p-6 mb-6">
          <button class="bg-white transition duration-300 hover:bg-gray-100 text-gray-800 py-2 px-4 border border-solid border-black mr-1">
            &#10004;
          </button>
          <div class="text-left">
            <p class="font-bold">№ 74687474 от 28.06.2021</p>
            <p>Оплачен. Заказ выполнен</p>
          </div>
          <div>
            1450 ₽
          </div>
          <img src="~/assets/images/icons/union.svg" alt="union">
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "personal",
  data() {
    return {
      country: this.country
    }
  },
  computed: {
    country() {
      return this.$store.state.country
    }
  }
}
</script>

<style scoped>

</style>

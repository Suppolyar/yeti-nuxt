<template>
  <section class="container mx-auto border-black border-t border-b text-black text-sm mb-6 mt-12">
    <div class="flex flex-col lg:grid grid-cols-2">
      <div class="grid grid-cols-3 gap-3 mb-12 lg:mb-0">
        <NuxtLink class="hover:text-gray-400 duration-300" to="#">Главная</NuxtLink>
        <NuxtLink class="hover:text-gray-400 duration-300" to="#">Продукты</NuxtLink>
        <NuxtLink class="hover:text-gray-400 duration-300" to="#">Доставка и оплата</NuxtLink>
        <NuxtLink class="hover:text-gray-400 duration-300" to="#">О нас</NuxtLink>
        <NuxtLink class="hover:text-gray-400 duration-300" to="#">World Eggs</NuxtLink>
        <NuxtLink class="hover:text-gray-400 duration-300" to="#">Сервис и помощь</NuxtLink>
      </div>
      <div class="flex flex-col md:flex-row justify-between lg:grid grid-cols-2 gap-3 justify-items-end lg:w-2/3 lg:ml-auto">
        <a class="hover:text-gray-400 duration-300" href="#">mail@mail.com</a>
        <a class="hover:text-gray-400 duration-300" href="#">+7 (3452) 602 428</a>
        <a class="hover:text-gray-400 duration-300 col-span-2" href="#">г. Москва, ул. Улица, 11, оф. 406</a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "footerVue"
}
</script>

<style scoped>

</style>

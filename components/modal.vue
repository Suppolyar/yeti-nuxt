<template>
  <div class="fixed z-10 inset-0 overflow-y-auto" aria-labelledby="modal-title" role="dialog" aria-modal="true">
    <div class="flex justify-center items-center min-h-screen pt-4 px-4 pb-20 text-center sm:block sm:p-0">
      <!--
        Background overlay, show/hide based on modal state.

        Entering: "ease-out duration-300"
          From: "opacity-0"
          To: "opacity-100"
        Leaving: "ease-in duration-200"
          From: "opacity-100"
          To: "opacity-0"
      -->
      <div class="fixed inset-0 bg-gray-500 bg-opacity-75 transition-opacity" aria-hidden="true"></div>

      <!-- This element is to trick the browser into centering the modal contents. -->
      <span class="hidden sm:inline-block sm:align-middle sm:h-screen" aria-hidden="true">&#8203;</span>

      <!--
        Modal panel, show/hide based on modal state.

        Entering: "ease-out duration-300"
          From: "opacity-0 translate-y-4 sm:translate-y-0 sm:scale-95"
          To: "opacity-100 translate-y-0 sm:scale-100"
        Leaving: "ease-in duration-200"
          From: "opacity-100 translate-y-0 sm:scale-100"
          To: "opacity-0 translate-y-4 sm:translate-y-0 sm:scale-95"
      -->
      <div class="inline-block align-bottom bg-white rounded-2xl text-left overflow-hidden shadow-xl transform transition-all sm:my-8 sm:align-middle sm:max-w-lg  border border-solid border-black px-9 pb-9">
        <div class="bg-white px-4 pt-5 pb-4 sm:p-6 sm:pb-4 ">
          <div class="text-center text-2xl mb-6">Вход на сайт</div>
        </div>
        <div>
          <label class=" tracking-wide text-gray-700 text-xs  mb-2" for="email-address-enter">
            Е-mail-адрес*
          </label>
          <input class="appearance-none block w-full bg-white text-gray-700 border border-black py-3 px-4 leading-tight focus:outline-none focus:bg-grey-100 focus:border-gray-500 border-solid" id="email-address-enter" type="email" placeholder="email@mail.ru">
        </div>
        <div class="mb-6">
          <label class=" tracking-wide text-gray-700 text-xs  mb-2" for="password">
            Пароль*
          </label>
          <input class="appearance-none block w-full bg-white text-gray-700 border border-black py-3 px-4 leading-tight focus:outline-none focus:bg-grey-100 focus:border-gray-500 border-solid" id="password" type="password" placeholder="Пароль">
        </div>
        <div class="flex flex-col mb-6">
          <a class="text-center opacity-70 hover:opacity-100 border-black transition duration-300" href="#">Регистрация</a>
          <a class="text-center opacity-70 hover:opacity-100 border-black transition duration-300" href="#">Забыли пароль</a>
        </div>
        <div class="text-center">
          <button class="w-2/3 !mx-auto text-uppercase bg-black text-base transition duration-300 hover:bg-opacity-80 text-white py-2 px-4 border border-solid border-black ml-3">
            вход
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "modal"
}
</script>

<style scoped>

</style>

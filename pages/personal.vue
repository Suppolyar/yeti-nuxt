<template>
  <section class="container mx-auto">
    <div class="text-black text-5xl text-center mb-6">Личный кабинет</div>
    <div class="text-2xl mb-6">Здравствуйте, Анна! Добро пожаловать в Ваш личный кабинет</div>
    <div class="xl:grid grid-cols-2 gap-x-6">
      <v-form v-model="valid">
        <div>Личные данные:</div>
        <div class="grid grid-cols-2 gap-x-6">
          <v-text-field
              v-model="firstname"
              :rules="nameRules"
              :counter="10"
              label="Имя"
              required
          ></v-text-field>
          <v-text-field
              v-model="lastname"
              :rules="nameRules"
              :counter="10"
              label="Фамилия"
              required
          ></v-text-field>
          <v-text-field
              v-model="email"
              :rules="emailRules"
              label="Почта"
              required
          ></v-text-field>
          <v-text-field
              v-model="tel"
              :type="tel"
              label="Телефон"
              required
          ></v-text-field>
        </div>
        <div>
          <v-select
              v-model="country"
              :items="country"
              label="Страна"
          ></v-select>
        </div>
        <div>
          <v-text-field
              v-model="city"
              label="Населенный пункт"
              required
          ></v-text-field>
        </div>
        <div class="grid grid-cols-2 gap-x-6">
          <v-text-field
              v-model="postcode"
              label="Почтовый индекс"
              required
          ></v-text-field>
          <v-text-field
              v-model="region"
              label="Область"
              required
          ></v-text-field>
        </div>
      </v-form>
      <div>
        <div class="mb-6">Заказы</div>
        <div class="flex flex-row justify-between items-center border border-black p-6">
          <v-btn
              class="mx-2"
              fab
              dark
              small
              color="primary"
          >
            <v-icon dark>
              mdi-check-bold
            </v-icon>
          </v-btn>
          <div class="text-left">
            <p class="font-bold">№ 74687474 от 28.06.2021</p>
            <p>Оплачен. Заказ выполнен</p>
          </div>
          <div>
            1450 ₽
          </div>
          <v-icon>
            mdi-chevron-down
          </v-icon>
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

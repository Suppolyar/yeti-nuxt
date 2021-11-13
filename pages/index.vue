<!--У меня возникают проблемы с Layout/default.vue,-->
<!--я не понимаю как правильно прикрепить футер и хидер, -->
<!--а так же правильно настроить роутинг между компонентами, -->
<!--в документации перекопался, но при компиляции, default.vue в-->
<!--.nuxt все равно перекампиливает и сбивает хидер и футер.-->
<!--надеюсь на вашу помощь Сенсей)-->

<!--Что бы посмотреть страничку мне приходиться закомментировать один-->
<!--компонент и раскомментировать другой-->

<template>
  <div>
    <header-vue></header-vue>
    <Nuxt/>
    <!--    <main-page></main-page>-->
    <!--    <about-page></about-page>-->
    <!--    <catalog></catalog>-->
    <products></products>
    <!--    <product-item></product-item>-->
    <footer-vue></footer-vue>
  </div>
</template>

<script>
import HeaderVue from "../components/headerVue";
import FooterVue from "../components/footerVue";
import Main from "./main";
import About from "./about";
import Products from "./products";
import Catalog from "./catalog";
import ProductItem from "./productItem";

export default {
  components: {ProductItem, Catalog, Products, About, Main, FooterVue, HeaderVue}
}
</script>

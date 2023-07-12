<template>
  <HeaderVue />
  <SliderVue />
  <ArticleVue />
  <ContactVue/>
  <FooterVue/>
</template>

<script>
import HeaderVue from './components/HeaderVue.vue'
import SliderVue from './components/SliderVue.vue'
import ArticleVue from './components/ArticleVue.vue'
import ContactVue from './components/ContactVue.vue'
import FooterVue from './components/FooterVue.vue'

export default {
  name: 'App',
  components: {
    SliderVue,
    HeaderVue,
    ArticleVue,
    ContactVue,
    FooterVue
  }
}
</script>

<style></style>

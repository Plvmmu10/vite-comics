<template>
  <header>
    <HeaderDC />
  </header>

  <main>
    <JumbotronDC />
    <MainDC />
    <div class="mainNav">
      <MainNavDC />
    </div>
  </main>

  <footer>
    <FooterDC />
  </footer>
</template>

<script>
import HeaderDC from './components/HeaderDC.vue';
import JumbotronDC from './components/JumbotronDC.vue';
import MainDC from './components/MainDC.vue';
import MainNavDC from './components/MainNavDC.vue';
import FooterDC from './components/FooterDC.vue';
export default {
  name: 'App',
  components: {
    HeaderDC,
    JumbotronDC,
    MainDC,
    MainNavDC,
    FooterDC
  }
}
</script>

<style lang="scss" scoped></style>
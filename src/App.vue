<template>
  <header>
    <HeaderDC />
  </header>

  <main>
    <MainDC />
    <div class="mainNav">
      <MainNavDC />
    </div>

  </main>
</template>

<script>
import HeaderDC from './components/HeaderDC.vue';
import MainDC from './components/MainDC.vue';
import MainNavDC from './components/MainNavDC.vue';
export default {
  name: 'App',
  components: {
    HeaderDC,
    MainDC,
    MainNavDC,
  }
}
</script>

<style lang="scss" scoped></style>
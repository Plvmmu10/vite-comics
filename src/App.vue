<template>
  <header>
    <HeaderDC />
  </header>

  <main>
    <MainDC />
  </main>
</template>

<script>
import HeaderDC from './components/HeaderDC.vue';
import MainDC from './components/MainDC.vue';
export default {
  name: 'App',
  components: {
    HeaderDC, MainDC,
  }
}
</script>

<style lang="scss" scoped></style>
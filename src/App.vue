<template>
  <header-item/>
  <default-layout><h2>Home Page</h2></default-layout>
</template>

<script>
import HeaderItem from './components/Layouts/components/Header.vue'
import DefaultLayout from './components/DefaultLayouts/DefaultLayout.vue';

export default {
  name: 'App',
  components: {
    HeaderItem,
    DefaultLayout
  }
}
</script>

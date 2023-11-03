<template>
  <AppHeader v-bind:appTitle="message" v-on:change="changeMessage"></AppHeader>
</template>

<script>
//import 컴포넌트 이름 from './컴포넌트 경로'
import AppHeader from './components/AppHeader.vue'

export default {
  components: {
    AppHeader
  },
  data() {
    return {
      message: '앱 헤더 컴포넌트'
    }
  },
  methods: {
    showAlert() {
      alert('hello')
    },
    changeMessage() {
      this.message = '제목 바꿔버렷';
    }
  }
}
</script>

<style scoped>

</style>
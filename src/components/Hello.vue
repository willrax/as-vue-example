<template>
  <div class="hello">
    <input v-model="message">

    <button @click="sendAlert">
      Alert
    </button>
  </div>
</template>

<script>
  export default {
    name: 'hello',

    props: ['defaultMessage'],

    data () {
      return {
        message: this.defaultMessage
      }
    },

    methods: {
      sendAlert () {
        alert(this.message)
      }
    }
  }
</script>

<style scoped>
  button {
    color: red;
  }
</style>

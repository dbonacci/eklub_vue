<template>
  <div class="register">
    <h1>Registrirajte se</h1>
    <input
      type="email"
      name="email"
      v-model="email"
      placeholder="email"/>
    <br>
    <input
      type="password"
      name="password"
      v-model="password"
      placeholder="password"/>
    <br>
    <button
      @click="register">
      Register
    </button>
  </div>
</template>

<script>
export default {
  data () {
    return {
      email: '',
      password: ''
    }
  },
  methods: {
    register () {
      console.log('register button was clicked', this.email, this.password)
    }
  }
}
</script>

<style scoped>
</style>

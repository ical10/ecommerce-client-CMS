<template>
  <div class="home">
    <LoginForm
    @login='login'/>
  </div>
</template>

<script>
// @ is an alias to /src
import LoginForm from '@/components/LoginForm.vue'

export default {
  name: 'Home',
  components: {
    LoginForm
  },
  methods: {
    login (payload) {
      this.$emit('login', payload)
    }
  }
}
</script>

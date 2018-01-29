<template>
    <div>
        <h1>Login</h1>
        <logo size="200"></logo>
    </div>
</template>

<script>
import logo from '../../components/logo'
export default {
  name: 'login',
  components: { logo },
  data () {
    return {
      email: '',
      password: ''
    }
  },
  methods: {
    login () {
      this.$store.dispatch('login', {
        email: this.email,
        password: this.password
      }).then(() => {
        this.$router.push('/objective/add')
      })
    }
  }
}
</script>

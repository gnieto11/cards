<template>
  <registration-form 
    @success="createdUser" />
</template>

<script>
  import RegistrationForm from '../components/RegistrationForm'
  export default {
    name: 'Registration',
    components: {
      RegistrationForm
    },
    methods: {
      createdUser () {
        this.$router.push({name: 'Login'})
      }
    }
  }
</script>

<style scoped>

</style>
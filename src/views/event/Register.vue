<template>
  <p>Register for the event here</p>
  <button @click="register">Regiser Me</button>
</template>

<script>


export default {
  props: ['event'],
  methods: {
    register() {
        // Cal to applicationIf registered then redirect ot even details
        this.$router.push({
            name: 'EventDetails'
        })
    }
  }
}
</script>

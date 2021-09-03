<template>
  <p>Register for the event here</p>
  <button @click="register">Register My Event</button>
</template>

<script>
export default {
  props: ['event'],
  methods: {
    register() {
      // call to API
      // If registered then redirect to event details
      this.$router.push({
        name: 'EventDetails',
      })
    },
  },
}
</script>

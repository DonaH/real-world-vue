<template>
  <div class="about">
    <h1>No such {{ resource }} can be found at this time.</h1>
    <router-link :to="{ name: 'EventList' }">Back to the home page</router-link>
  </div>
</template>

<script>
export default {
  props: {
    resource: {
      type: String,
      required: true,
      default: 'page',
    },
  },
}
</script>

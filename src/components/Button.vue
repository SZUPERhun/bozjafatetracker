<template>
  <div>
    <b-button variant="warning" @click="startTimer()">{{ msg }}</b-button>
  </div>
</template>

<script>
export default {
  name: 'Button',
  props: ['msg'],
  methods: {
    startTimer: function() {
      this.$emit('clicked');
    },
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>

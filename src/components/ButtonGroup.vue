<template>
  <div>
    <Button @clicked="onClicked" :msg="buttonMessage"/> <br>
    <span v-if="timeStart">
      <Timer />
    </span>
    <br>
  </div>
</template>

<script>
import Button from './Button.vue';
import Timer from './Timer.vue';
export default {
  name: 'ButtonGroup',
  data() {
      return {
          start: false,
      }
  },
  computed: {
    timeStart () {
      return this.start;
    },
    buttonMessage() {
      if (this.start) {
        return "Stop timer";
      }

      return "Start timer";
    }
  },
  methods: {
    onClicked: function() {
      this.start = !this.start;
    }
  },
  components: {
    Button,
    Timer,
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>

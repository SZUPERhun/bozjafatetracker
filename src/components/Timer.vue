<template>
  <div>
    <vue-countdown-timer
      class="countdown"
      @start_callback="startCallBack('event started')"
      @end_callback="endCallBack('event ended')"
      :start-time="startTime"
      :end-time="end_time?end_time:endTime"
      :interval="1000"
      :end-text="'Fate chain is spawnable'">
      <template slot="countdown" slot-scope="scope">
        <span>{{scope.props.hours}}:{{scope.props.minutes}}:{{scope.props.seconds}}</span>
      </template>
    </vue-countdown-timer>
  </div>
</template>

<script>
export default {
  name: 'Timer',
  data() {
      return {
          startTime: (new Date).getTime(),
          endTime: (new Date).getTime()+1000*60*60,
      }
  },
  methods: {
    startCallBack: function(x) {
      console.log(x);
    },
    endCallBack: function(x) {
      console.log(x);
    },
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .countdown {
    color: red !important;
    font-size: 120%;
    font-weight: bold;
  }
</style>

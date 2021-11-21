<template>
  <b-container>
    <b-row>
      <b-col>
        <ButtonGroup/>
        <span class="big">The Shadow of Death's Hand</span>
      </b-col>
      <b-col>
        <ButtonGroup/>
        <span class="big">The Baying of the Hound(s)</span>
      </b-col>
      <b-col>
        <ButtonGroup/>
        <span class="big">All Pets Are off</span> <span class="grey">-> Kill It with Fire</span>
      </b-col>
      <b-col>
        <ButtonGroup/>
        <span class="big">More Machine Now than Man</span> <span class="grey">-> Vigil for the Lost</span>
      </b-col>
    </b-row>
    <b-row>
      <b-col>
        <ButtonGroup/>
        <span class="big">Unicorn Flakes</span> <span class="grey">-> The Final Furlong</span>
      </b-col>
      <b-col>
        <ButtonGroup/>
        <span class="big">The Fires of War</span> <span class="grey">-> Patriot Games</span>
      </b-col>
      <b-col>
        <ButtonGroup/>
        <span class="big">Red (Chocobo) Alert</span> <span class="grey">-> The Hunt for Red Choctober</span>
      </b-col>
    </b-row>
    <b-row>
      <b-col>
        <ButtonGroup/>
        <span class="big">I'm a Mechanical Man</span> <span class="grey">-> Rise of the Robots</span>
      </b-col>
      <b-col>
        <ButtonGroup/>
        <span class="big">Trampled under Hoof</span> <span class="grey">-> Where Strode the Behemoth</span>
      </b-col>
      <b-col>
        <ButtonGroup/>
        <span class="big">For Absent Friends</span> <span class="grey">-> Of Steel and Flame -> Metal Fox Chaos</span>
      </b-col>
    </b-row>
    <img src="../assets/bozjaguide.webp" alt="bozja guide" style='height: 100%; width: 100%; object-fit: contain'>
  </b-container>
</template>

<script>
import ButtonGroup from './ButtonGroup.vue';

export default {
  name: 'Index',
  components: {
    ButtonGroup,
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .row {
    margin-bottom: 100px;
  }
  .grey {
    color: grey;
  }
  .big {
    font-size: 120%;
    font-weight: bold;
  }
</style>

<template>
  <div class="card">
    <div class="card-image" :style="{'background-image': 'url(./img/'+imgMate+')'}">
    </div>

    <div class="card-text">
      <span class="job">{{jobTitle}}</span>
      <h2>{{firstName+' '+lastName}}</h2>
      <p>{{verbatim}}</p>
    </div>
    <TeamTechno :stack="stack" />
  </div>
</template>

<script>

import TeamTechno from './TeamTechno'

export default {
  name: "TeamCard",
  created() {},
  components: {
    TeamTechno,
  },
  data:() => ({

  }),
  props: {
    "firstName": {
      type: String,
    },
    "lastName": {
      type: String,
    },
    "verbatim": {
      type: String,
    },
    "jobTitle": {
      type: String,
    },
    "imgMate": {
      type: String,
    },
    "stack": {
      type: Array,
    },
  },
  methods: {},
};
</script>

<style scoped>
  @import "../assets/css/card_styles.css";
</style>
<template>
  <div>
    <div class="card-stats">
      <div class="stat" v-for="(techno, index) in stack" :key="index">
        <div class="techno">{{techno.label}}</div>
        <div class="level">{{leveling(techno.level)}}</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TeamTechno",
  created() {},
  data() {
    return {};
  },
  props: {
    stack: {
      type: Array,
    },
  },
  methods: {
    leveling(data){
      return '⭐'.repeat(data)
    }
  },
};
</script>

<style scoped>
    @import "../assets/css/card_styles.css";
</style>
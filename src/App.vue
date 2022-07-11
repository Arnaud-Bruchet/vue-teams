<template>
  <div id="app">
    <TeamCard v-for="(teamMate, index) in teams" :key="index" />
  </div>
</template>

<script>

import teams from './assets/js/teams.js'
import TeamCard from './components/TeamCard'

export default {
  name: 'App',
  data: () => ({
    teams
  }),
  components: {
    TeamCard,
  }
}
</script>

<style>

</style>

<template>
  <div id="app">
    <TeamCard 
      v-for="(teamMate, index) in teams" 
      :key="index" :firstName="teamMate.firstName"
      :lastName="teamMate.lastName" 
      :verbatim="teamMate.verbatim" 
      :jobTitle="teamMate.jobTitle"
      :imgMate="teamMate.profilePic"
      :stack="teamMate.stack"
    />
  </div>
</template>

<script>

import TeamCard from './components/TeamCard'
import {teams} from './assets/js/teams.js'

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

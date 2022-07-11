<template>
  <div>
    <div class="card">
      <div class="card-image"></div>
      <div class="card-text">
        <span class="job">Full Stack 🎉</span>
        <h2>FirstName & LastName</h2>
        <p>verbatim</p>
      </div>
      <div class="card-stats">
        <div class="stat">
          <div class="techno">Techno</div>
          <div class="level">⭐⭐⭐⭐</div>
        </div>
        <div class="stat border">
          <div class="techno">Techno</div>
          <div class="level">⭐⭐⭐</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TeamCard",
  created() {},
  data:() => ({

  }),
  props: {},
  methods: {},
};
</script>

<style scoped>
@import "../assets/css/card_styles.css"
</style>
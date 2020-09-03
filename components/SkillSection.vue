<template>
  <div class="skill-section">
    <div class="skill-title">{{ title }}</div>
    <div class="skill-list">
      <b-table borderless :fields="fields" :items="skills"></b-table>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: { type: String, required: true },
    fields: { type: Array, required: true },
    skills: { type: Array, required: true },
  },
}
</script>

<style lang="sass" scoped>
.skill-section
  background-color: rgba(0, 0, 0, 0.1)
  border-radius: 5px
  padding: 10px
  margin-bottom: 10px

  .skill-title
    font-size: 24px
    font-weight: 700

  .skill-list
    margin-bottom: 10px
    font-size: 20px
</style>

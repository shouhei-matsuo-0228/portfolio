<template>
  <div class="content-section">
    <div class="heading">{{ heading }}</div>
    <slot></slot>
  </div>
</template>

<script>
export default {
  props: {
    heading: { type: String, required: true },
  },
}
</script>

<style lang="sass" scoped>
.content-section
  padding: 30px
  margin-bottom: 30px
  .heading
    font-weight: 700
    font-size: 36px
    margin-bottom: 10px
</style>

<template>
  <div>
    <b-jumbotron :header="header">
      <p>{{ subText }}</p>
    </b-jumbotron>
  </div>
</template>

<script>
export default {
  props: {
    header: { type: String, required: true },
    subText: { type: String, required: false, default: null },
  },
}
</script>

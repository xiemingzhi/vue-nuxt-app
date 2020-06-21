<template>
  <div>Displaying comments for {{ key }}</div>
</template>

<script>
export default {
  data() {
    return {
      key: this.$route.params.slug
    }
  }
}
</script>

<style lang="scss" scoped></style>

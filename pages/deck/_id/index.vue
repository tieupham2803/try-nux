<template>
  <h1>my deck id {{ $route.params.id }} is active</h1>
</template>
<script>
export default {
  validate({ params }) {
    return /^[0-9]{9,12}$/.test(params.id)
  },
}
</script>

<template>
  <div :class="$style.parent">
    <p>parent</p>
    <child></child>
  </div>
</template>

<script>
import Child from './Child'
export default {
  components: { Child }
}
</script>

<style module>
.parent {
  color: red;
}
</style>

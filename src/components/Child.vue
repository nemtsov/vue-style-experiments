<template>
  <div :class="$style.child">
    <p>child</p>
    <grand-child></grand-child>
  </div>
</template>

<script>
import GrandChild from './GrandChild'
export default {
  components: { GrandChild }
}
</script>

<style module>
.child {
  color: green;
}
</style>

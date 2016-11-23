<template>
  <div :class="$style.parent">
    <p>parent</p>
    <child :userStyle="{message: $style.message}"></child>
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

.message {
  composes: message from './GrandChild.css';
  padding: 100px;
}
</style>

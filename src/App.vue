<template>
  <div id="app">
    <p>app</p>
    <child :class="$style.override"></child>
  </div>
</template>

<script>
import Child from './components/Child'
export default {
  components: { Child }
}
</script>

<style module>
.override {
  color: purple;
}
</style>

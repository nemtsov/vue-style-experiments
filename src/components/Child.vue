<template>
  <div :class="$style.child">
    <p>child</p>
    <grand-child :userStyle="{message: userStyle.message}"></grand-child>
  </div>
</template>

<script>
import GrandChild from './GrandChild'
export default {
  components: { GrandChild },
  props: [ 'userStyle' ]
}
</script>

<style module>
.child {
  color: green;
}
</style>

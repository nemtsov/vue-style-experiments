<template>
  <div :class="$style.grandchild">
    <p :class="userStyle.message">grandchild</p>
  </div>
</template>

<script>
export default {
  props: [ 'userStyle' ]
}
</script>

<style module>
.grandchild {
  color: blue;
}

.message {
  padding: 10px;
  border: 2px dashed #ccc;
}
</style>

<template>
  <div class="not-found">
    <strong>404</strong>
  </div>
</template>

<script>
export default {
  name: "NotFound"
};
</script>

<style scoped lang="scss">
@mixin user-select($select) {
  -webkit-touch-callout: #{$select};
  @each $pre in -webkit-, -moz-, -ms-, -o-, -khtml- {
    #{$pre + user-select}: #{$select};
  }
  #{user-select}: #{$select};
}
.not-found {
  text-align: center;
  font-size: 12em;
  color: #879bc6;
  @include user-select(none);
}
</style>

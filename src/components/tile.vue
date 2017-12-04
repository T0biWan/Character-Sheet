<template>
  <div class="tile is-parent">
    <div class="tile is-child">
      <slot></slot>
    </div>
  </div>
</template>

<script>
  export default {
    name: "tile",
  }
</script>

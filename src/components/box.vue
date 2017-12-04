<template>
  <div class="box has-text-centered">
    <h2 class="title is-4">{{title}}</h2>
    <p class="">{{value}}</p>
  </div>
</template>

<script>
  export default {
    name: "box",
    props: {
      title: this.title,
      value: this.value
    },
  }
</script>

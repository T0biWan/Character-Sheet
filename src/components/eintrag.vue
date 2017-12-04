<template>
  <div>
    <h6 class="title is-5">{{title}}</h6>
    <p><slot></slot></p>
  </div>
</template>

<script>
export default {
  name: "eigenschaft",
  props: {
    title: this.title,
  },
}
</script>

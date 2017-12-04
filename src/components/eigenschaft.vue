<template>
  <div>
    <h6>{{title}}</h6>
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

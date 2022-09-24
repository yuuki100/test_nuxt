<template lang="pug">
  .container
    h1.title
      | {{myName}}
    //-  | {{$store.state.message}}

    a(href="/") back
</template>

<script>
export default {
  computed: {
    myName() {
      console.log(this)
      console.log(this.$store)

      return "hoge"
    }
  },
}

</script>

<style lang="scss">
.red {
  color: red
}

h1 {
  background-color: black;
  color: white;
}
</style>


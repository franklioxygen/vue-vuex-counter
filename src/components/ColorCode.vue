<template>
  <div>
  <input placeholder="Enter color code" type="text" v-model="colorCode">
</div>
</template>

<script>
export default {
    name: 'color code',
    computed: {
    colorCode: {
      get() {
        return this.$store.state.colorCode
      },
      set(newValue) {
        this.$store.commit('setColorCode', newValue)
      }
    }
  }
}
</script>

<style>

</style>
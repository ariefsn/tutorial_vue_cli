<template>
  <div>
    <div>Child Value: {{ newValue }}</div>
    <input type="text" v-model="newValue">
  </div>
</template>

<script>
export default {
  props: {
    value: {
      type: [String],
      default: ''
    }
  },
  data () {
    return {
      newValue: this.value
    }
  },
  watch: {
    newValue (v) {
      this.$emit('input', v)
    }
  }
}
</script>

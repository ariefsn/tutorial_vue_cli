<template>
  <div>
    <div>Parent Value: {{ value }}</div>
    <VModelChild v-model="value"/>
  </div>
</template>

<script>
import VModelChild from '../components/VModelChild'

export default {
  components: {
    VModelChild
  },
  data () {
    return {
      value: 'Halooo'
    }
  },
  methods: {
    updateNilai (nilaiBaru) {
      this.value = nilaiBaru
    }
  }
}
</script>

<template>
  <div>{{ teks }}</div>
</template>

<script>
export default {
  props: {
    teks: {
      type: String,
      default: 'Ini adalah komponen teks'
    }
  }
}
</script>

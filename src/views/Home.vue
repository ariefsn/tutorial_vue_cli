<template>
  <div>
    <KomponenTeks teks="Halooo"/>
    <KomponenTeks/>
    <KomponenTeks teks="Teks ini kita set melalui props"/>
  </div>
</template>

<script>
import KomponenTeks from '@/components/KomponenTeks.vue'

export default {
  name: 'Home',
  components: {
    KomponenTeks
  }
}
</script>

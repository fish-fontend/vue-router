<template>
  <div>
    It is common component!
    <router-link to="/">
      <a>to /</a>
    </router-link>
  </div>
</template>

<script>
var thisName = 'Common.vue'

export default {
  created () {
    console.log(`created ${thisName}`)
  },
  mounted () {
    console.log(`mounted ${thisName}`)
  },
  updated () {
    console.log(`updated ${thisName}`)
  },
  destroyed () {
    console.log(`destoryed ${thisName}`)
  }
}
</script>

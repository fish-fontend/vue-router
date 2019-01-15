<template>
  <div>
    <h1>It it vue</h1>
    <Links></Links>
    <HelloVue></HelloVue>
  </div>
</template>

<script>
import HelloVue from '@/components/HelloVue.vue'
import Links from '@/components/Links.vue'

export default {
  components: {
    HelloVue,
    Links
  }
}
</script>

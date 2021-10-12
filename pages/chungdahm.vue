<template>
  <div>
      Hi
      <NuxtLink :to="{ name: 'chungdahm-abc' }">Parent</NuxtLink>
      <nuxt-child />
  </div>
</template>

<script>
export default {
  head () {
    return {
      title: 'Hello Chungdahm',
      meta: [
        { charset: 'utf-8' },
        { name: 'viewport', content: 'width=device-width, initial-scale=1' },

        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        { hid: 'description', name: 'Hi Chungdahm', content: 'Hello This is Louis.' }
      ]
    }
  },
  meta: {
    theme: 'blue'
  }
}
</script>

<style>

</style>
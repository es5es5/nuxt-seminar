<template>
  <div>
    <h1>Parent</h1>
    <p>
      Checkout
    </p>
    <NuxtLink tag="p" :to="{ name: 'parent-blue' }">Blue page</NuxtLink>
    <NuxtLink tag="span" :to="{ name: 'parent-childId', params: { childId } }">
      Go to {{ childId }} Child
    </NuxtLink>
    <input type="text" v-model="childId">

    <NuxtChild />
  </div>
</template>

<script>
export default {
  name: 'Parent',
  data () {
    return {
      childId: 'red'
    }
  },
  meta: {
    theme: 'orange'
  }
}
</script>

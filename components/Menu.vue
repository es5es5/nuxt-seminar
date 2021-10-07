<template>
  <div>
    <div class="nav horizontal-align">
        <NuxtLink class="nav-item" to="/">Home</NuxtLink>
        <NuxtLink class="nav-item" :to="{ name: 'about' }">About</NuxtLink>
        <NuxtLink class="nav-item" :to="{ path: '/parent' }">Parent page</NuxtLink>
        <NuxtLink class="nav-item" :to="{ name: 'chungdahm' }">ChungDahm</NuxtLink>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>
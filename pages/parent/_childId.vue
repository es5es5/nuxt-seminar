<template>
  <div>
      <p>this.$route.params.childId: <b>{{ _childId }}</b></p>
  </div>
</template>

<script>
export default {
    name: 'Child',
    computed: {
        _childId () {
           return this.$route.params.childId
        }
    },
    meta() {
        return {
                theme: () => {
            return 'this._childId'
            }
        }
    }
}
</script>

<style>

</style>
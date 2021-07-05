<template>
  <div>
    <Nuxt />
  </div>
</template>

<script>
export default {
  methods: {
    color() {
      console.log('test')
    }
  },
  mounted () {
    this.color();
  },
}
</script>

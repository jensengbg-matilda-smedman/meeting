<template>
  <div id="app">
    <header>
      
    </header>
    <router-view />
  </div>
</template>

<script>
export default {
  name: 'App',
  beforeMount() {
    this.$store.dispatch("fetchBackend")
  }
}
</script>


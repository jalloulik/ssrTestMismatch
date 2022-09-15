<template>
  <div>
    <div>This is displayed on the server and client</div>
    <div v-show="isMobile">
      This is displayed on mobile but always on server
    </div>
  </div>
</template>

<script>
export default {
  name: 'SeoDependencyMismatchMobileFix',
  data() {
    return {
      isMobile: true,
    }
  },
  head: {
    title: 'seoDependencyMismatchMobileFix',
  },
  beforeMount() {
    // This is to demonstrate the case where the page loads on desktop on the client
    this.isMobile = false
  },
}
</script>

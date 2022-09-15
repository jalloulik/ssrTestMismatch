<template>
  <div>
    <div>This is displayed on the server and client</div>
    <div v-if="trueInClient">This is displayed on the client only</div>
  </div>
</template>

<script>
export default {
  name: 'SsrWithMismatch',
  data() {
    return {
      trueInClient: false,
    }
  },
  head: {
    title: 'ssrWithMismatch',
  },
  beforeMount() {
    this.trueInClient = true
  },
}
</script>

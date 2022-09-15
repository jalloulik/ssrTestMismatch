<template>
  <div>
    <div>This is displayed on the server and client</div>
    <client-only>
      <div v-if="trueInClient">This is displayed on the client only</div>
    </client-only>
  </div>
</template>

<script>
export default {
  name: 'SsrWithMismatchWithClientOnly',
  data() {
    return {
      trueInClient: false,
    }
  },
  head: {
    title: 'ssrWithMismatchWithClientOnly',
  },
  beforeMount() {
    this.trueInClient = true
  },
}
</script>

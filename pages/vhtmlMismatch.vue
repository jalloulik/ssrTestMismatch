<template>
  <div>
    <div>This is displayed on the server and client</div>
    <ds-title v-html="vhtmlToDisplay" />
  </div>
</template>

<script>
import DsTitle from '~/components/DsTitle.vue'
export default {
  name: 'VhtmlMismatch',
  components: {
    DsTitle,
  },
  head: {
    title: 'vhtmlMismatch',
  },
  computed: {
    vhtmlToDisplay() {
      return 'Hello <br> everyone'
    },
  },
}
</script>

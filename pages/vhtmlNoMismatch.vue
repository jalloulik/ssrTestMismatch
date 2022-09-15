<template>
  <div>
    <div>This is displayed on the server and client</div>
    <ds-title is-vhtml v-html="vhtmlToDisplay" />
  </div>
</template>

<script>
import DsTitle from '~/components/DsTitle.vue'
export default {
  name: 'VhtmlNoMismatch',
  components: {
    DsTitle,
  },
  head: {
    title: 'vhtmlNoMismatch',
  },
  computed: {
    vhtmlToDisplay() {
      return 'Hello <br> everyone'
    },
  },
}
</script>

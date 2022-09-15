<template>
  <div>
    <div>This is displayed on the server and client</div>
    <ds-title-mismatch-slots-default v-html="vhtmlToDisplay" />
  </div>
</template>

<script>
import DsTitleMismatchSlotsDefault from '~/components/DsTitle.vue'
export default {
  name: 'VhtmlSlotsDefaultMismatch',
  components: {
    DsTitleMismatchSlotsDefault,
  },
  head: {
    title: 'vhtmlSlotsDefaultMismatch',
  },
  computed: {
    vhtmlToDisplay() {
      return 'Hello <br> everyone'
    },
  },
}
</script>

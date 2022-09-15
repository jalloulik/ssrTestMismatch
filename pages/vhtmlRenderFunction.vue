<template>
  <div>
    <div>This is displayed on the server and client</div>
    <ds-title-render-function v-html="vhtmlToDisplay" />
  </div>
</template>

<script>
import DsTitleRenderFunction from '~/components/DsTitleRenderFunction'
export default {
  name: 'VhtmlRenderFunction',
  components: {
    DsTitleRenderFunction,
  },
  head: {
    title: 'vhtmlRenderFunction',
  },
  computed: {
    vhtmlToDisplay() {
      return 'Hello <br> everyone'
    },
  },
}
</script>

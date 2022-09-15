<template>
  <div v-if="!isVhtml">
    <slot />
  </div>
  <div v-else />
</template>

<script>
export default {
  name: 'DsTitle',
  props: {
    isVhtml: Boolean,
  },
}
</script>

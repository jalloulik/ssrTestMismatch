<template>
  <div v-if="$slots.default">
    <slot />
  </div>
  <div v-else />
</template>

<script>
export default {
  name: 'DsTitleMismatchSlotsDefault',
}
</script>

<template>
  <div>
    <AppHeader />
    <slot />
    <NuxtPage />
    <AppFooter />
  </div>
</template>



<script>
export default {
  name: 'DefaultLayout',
}
</script>

  <style scoped>
  /* Layout-specific styles */
  </style>
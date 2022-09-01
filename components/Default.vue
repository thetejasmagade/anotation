<template>
  <section>
    <Sidebar v-if="!$device.isMobile"/>
    <MobileSidebar v-else />
  </section>
</template>

<script>
export default {

}
</script>

<style>

</style>
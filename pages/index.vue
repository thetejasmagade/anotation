<template>
  <div>
    <Default />
    <v-main>
      <Navbar v-if="!$device.isMobile"/>
      Java, vuesdvsvsvd
    </v-main>
  </div>
</template>

<script>
import MobileSidebar from '~/components/MobileSidebar.vue';
import Default from '~/components/Default.vue';
export default { components: { MobileSidebar, Default } };
</script>

<style>
</style>
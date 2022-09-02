<template>
  <div>
    <Default />
    <v-main>
      <Navbar v-if="$device.isMobile==false"/>
      <main class="px-12 py-32" id="content">
        <div id="div">
        <h1 id="h1" v-contenteditable:heading="isEnabled" v-model="heading"></h1>
        <p id="data" v-contenteditable:data="isEnabled" v-model="data"></p>

        <component is="p" id="data" v-contenteditable:data="isEnabled" v-model="data"></component>
        </div>
      </main>
    </v-main>
  </div>
</template>

<script>
import MobileSidebar from '~/components/MobileSidebar.vue';
import Default from '~/components/Default.vue';
export default { 
  data() {
    return {
      isEnabled: true,
      heading: "Heading",
      data: "",
    }
  },
  components: { MobileSidebar, Default } 
};

</script>

<style>
  * {
    line-height: 1.5;
    font-family: ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol";
    -webkit-font-smoothing: auto;
    font-weight: 500;
    font-size: 14px;
  }

  #content {
    line-height: 1.5;
    font-family: ui-sans-serif;
    -webkit-font-smoothing: auto;
    width: 100%;
    justify-content: center;
    z-index: 3;
    flex-shrink: 0;
    box-sizing: border-box;
  }

  #h1 {
    font-size: 40px;
    color: #37352F;
    width: 100%;
    white-space: pre-wrap;
    word-break: break-word;
    caret-color: rgb(55, 53, 47);
    padding: 10px 0px;
    font-weight: 700;
    line-height: 1.2;
    background: transparent;
    border: none;
  }

  #div {
    max-width: 700px;
    width: 100%;
    margin: auto;
  }

  [contenteditable] {
  outline: 0px solid transparent;
}
</style>
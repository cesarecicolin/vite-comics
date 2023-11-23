<script>
import AppHeader from "./components/AppHeader.vue";
import  AppContent from "./components/AppContent.vue"
import AppInfo from "./components/AppInfo.vue"
export default {
  components: {
    AppHeader,
    AppContent,
    AppInfo
  }
}

</script>

<template>
  
    
    <AppHeader />
    <AppContent />
    <AppInfo />
</template>

<style lang="scss">
@use "./style/general.scss";

</style>

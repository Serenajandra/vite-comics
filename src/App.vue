<script>
import AppTeamTitansBanner from "./components/AppTeamTitansBanner.vue";
import AppHeader from "./components/AppHeader.vue";
import AppSectionBlack from "./components/AppSectionBlack.vue";
import AppFooter from './components/AppFooter.vue';
import AppBlueNav from "./components/AppBlueNav.vue";

export default{
    components: {
    AppHeader,
    AppTeamTitansBanner,
    AppSectionBlack,
    AppBlueNav,
    AppFooter,
}
  }

</script>

<template>
<AppHeader />
<AppTeamTitansBanner />
<AppSectionBlack />
<AppBlueNav />
<AppFooter />
</template>

<style lang="scss">
@use "./styles/general.scss" as *;
@use "./styles/partials/mixins.scss" as *;
@use "./styles/partials/variabiles.scss" as*;
</style>

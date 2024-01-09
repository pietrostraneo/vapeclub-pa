<script>
import AppMenu from "./components/AppMenu.vue"
import AppJumbo from "./components/AppJumbo.vue"
import BuyPod from "./components/BuyPod.vue"
import Reviews from "./components/Reviews.vue"
export default {
  components: {
    AppMenu,
    AppJumbo,
    BuyPod,
    Reviews
  }
}
</script>
<template lang="">
  <div>
    <AppMenu />
    <BuyPod />
    <AppJumbo />
  </div>
</template>
<style lang="scss" scoped>
@use './styles/generals.scss';
@use './styles/partials/variables' as *;
</style>
<template>
  <div id="app">
    <HeaderComponent/>
    <InfoComponent/>
    <TeListUsers/>
    <PriceComponent/>
    <SubscribeComponent/>
    <FooterComponent/>
  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'
import InfoComponent from './components/InfoComponent.vue'
import TeListUsers from './components/TeListUsers.vue'
import PriceComponent from './components/PriceComponent.vue'
import SubscribeComponent from './components/SubscribeComponent.vue'
import FooterComponent from './components/FooterComponent.vue'

export default {
  name: 'App',
  components: {
    HeaderComponent, InfoComponent, TeListUsers, PriceComponent, SubscribeComponent, FooterComponent
  }
}
</script>

<style lang="scss">
* {
    margin: 0;
    padding: 0;
}
a {
    text-decoration: none;
}
body {
    font-family: "Jost", sans-serif;
    overflow-x: hidden;
}
summary {
    display: block;
}
summary::-webkit-details-marker {
    display: none;
}
.center {
    padding-left: calc(50% - 610px);
    padding-right: calc(50% - 610px);
}
</style>

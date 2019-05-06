<template>
  <div class="t-fixed" id="app">
    <Header class="t-fixed__header">
      <template v-slot:label><span class="o-brand">Stock Advisor</span></template>
    </Header>
    <main class="t-fixed__content">
      <StockPage></StockPage>
    </main>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

import StockPage from './components/pages/StockPage.vue';
import Header from './components/components/Header.vue';

@Component({
  components: {
    Header,
    StockPage,
  },
})
export default class App extends Vue {
}
</script>

<style lang="scss">
@import "./styles/site.scss";
</style>

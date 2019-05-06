<template>
  <ZoomReveal v-bind:isRevealed="!!stock">
    <Section class="h-t-center">
      Stock search
      <!-- <app-stock-search (selectionChange)="onSelectionChange($event)"></app-stock-search> -->
    </Section>
    <Section>
      <Card>
        <template v-slot:header>
            Header
            <!-- <app-stock-header [stock]="stock"></app-stock-header> -->
        </template>
        Content
        <!-- <app-stock-report [stock]="stock"></app-stock-report> -->
      </Card>
    </Section>
  </ZoomReveal>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';
import { Stock } from '../../models/models';
import ZoomReveal from '../layouts/ZoomReveal.vue';
import Card from '../components/Card.vue';
import Section from '../components/Section.vue';

@Component({
  components: {
    ZoomReveal,
    Card,
    Section,
  },
})
export default class StockPage extends Vue {
  @Prop() public stock!: Stock;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>

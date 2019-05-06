<template>
    <div class="l-zoom-reveal" v-bind:class="{ 'is-revealed': isRevealed }">
        <slot></slot>
    </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class ZoomReveal extends Vue {
    @Prop() public isRevealed: boolean = false;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>

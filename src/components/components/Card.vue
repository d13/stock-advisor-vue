<template>
    <div class="c-card">
        <header class="c-card__header"><slot name="header"></slot></header>
        <div class="c-card__content">
            <slot></slot>
        </div>
    </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Section extends Vue {}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>

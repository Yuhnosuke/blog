<template>
    <div class="container">
        <LayoutHeader />
        <Nuxt />
        <LayoutFooter />
    </div>
</template>

<script lang="ts">
import Vue from 'vue';
import LayoutHeader from '../components/organisms/LayoutHeader.vue';
import LayoutFooter from '../components/organisms/LayoutFooter.vue';

export default Vue.extend({
    components: {
        LayoutHeader,
        LayoutFooter,
    }
})
</script>

<style scoped>
    * {
        padding: 0;
        margin: 0;
        font-family: sans-serif;
        background-color: #f9f9f9;
    }
    
</style>
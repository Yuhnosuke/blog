<template>
    <div class="text">{{value}}</div>
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
    name: 'BaseText',
    props: {
        value: {
            type: String,
            required: true,
        },
    }
})
</script>

<style scoped>
    .text {
        margin: 4px 8px;
        padding: 4px 8px;
    }

</style>
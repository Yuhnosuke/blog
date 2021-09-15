<template>
    <button type="button">
        {{label}}
    </button>
    
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
    name: 'BaseButton',
    props: {
        label: {
            type: String,
            required: true,
        }
    }
})
</script>

<style scoped>

</style>
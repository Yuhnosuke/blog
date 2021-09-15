<template>
    <div class="footer">
        <BaseText class="footer__legal-message" :value="legalMessage"/>
    </div>
</template>
<script lang="ts">
import Vue from 'vue';
import BaseText from '../atmos/BaseText.vue';

export default Vue.extend({
    name: 'LayoutFooter',
    components: {
        BaseText,
    },
    data: function() {
        return {
            legalMessage: '© 2021 Yuhnosuk Hashimoto All Rights Reserved.'
        }
    },
})
</script>

<style scoped>
    .footer {
        position: absolute;
        width: 100%;
        bottom: 0;
    }

    .footer__legal-message {
        text-align: center;
    }
</style>
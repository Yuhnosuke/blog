<template>
    <div class="header">
        <div class="header__container">
            <BaseText class="header__title" value="Blogy"/>
            <ul class="header__items">
                <li class="header_item"><BaseText
                    value="About"
                    />
                </li>
                <li class="header_item"><BaseText
                    value="Contact"
                    />
                </li>
            </ul>
        </div>
    </div>
</template>

<script lang="ts">
import Vue from 'vue';
import BaseText from '../atmos/BaseText.vue';

export default Vue.extend({
    name: 'LayoutHeader',
    components: {
        BaseText,
    }
})
</script>

<style scoped>
    .header {
        background-color: #f9f9f9;
    }
    .header__container {
        display: flex;
        flex-direction: row;
        justify-content: flex-end;
        width: 960px;
        margin: 0 auto;
    }
    @media screen and (max-width: 480px) {
        .header__container {
            width: 360px;
        }
    }
    
    .header__title {
        
        margin: auto;
        margin-left: 32px;
    }

    ul.header__items {
        display: flex;
        list-style-type: none;
    }

    
</style>
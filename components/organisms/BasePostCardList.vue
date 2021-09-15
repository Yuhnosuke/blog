<template>
    <div class="post-card-list-container">
        <div v-for="post in posts" :key=post._id>
            <BaseText :value="post.title"/>
            <BaseText :value="post.category"/>
            <BaseButton :label="buttonLabel"/>
            <BaseDivider />
        </div>
    </div>
    
</template>

<script lang="ts">
import Vue from 'vue';
import BaseText from '../atmos/BaseText.vue';
import BaseButton from '../atmos/BaseButton.vue';
import BaseDivider from '../atmos/BaseDivider.vue';

export default Vue.extend({
    name: 'BasePostCardList',
    components: {
        BaseText,
        BaseButton,
        BaseDivider,
    },
    data: function() {
        return {
            posts: {
                '1': {
                    _id: '1',
                    title: 'test title 1',
                    category: 'test category 1',
                },
                '2': {
                    _id: '2',
                    title: 'test title 2',
                    category: 'test category 2',
                },
                '3': {
                    _id: '3',
                    title: 'test title 3',
                    category: 'test category 3',
                },
            },
            buttonLabel: 'Read More...',
        }
    }
})
</script>

<style scoped>

</style>
<template>
    <v-navigation-drawer :model-value="props.drawer" location="left" temporary>
        <v-list :items="items"></v-list>
    </v-navigation-drawer>
</template>

<script setup>
import { ref } from 'vue';

const items = ref([
    {
        title: 'Login',
        value: 'login',
        path: '/login',
    },
    {
        title: 'Bar',
        value: '/bar',
        path: '/bar'
    },
    {
        title: 'Fizz',
        value: '/fizz',
        path: '/fizz'
    },
    {
        title: 'Buzz',
        value: '/buzz',
        path: '/buzz',
    },
]);

const props = defineProps({
    drawer: Boolean,
})
</script>

<style lang="scss" scoped></style>
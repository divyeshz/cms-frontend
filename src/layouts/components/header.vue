<template>
    <v-app-bar color="primary" prominent>
        <v-app-bar-nav-icon variant="text" @click.stop="drawer = !drawer"></v-app-bar-nav-icon>

        <v-toolbar-title>My files</v-toolbar-title>

        <v-spacer></v-spacer>

        <v-btn variant="text" icon="mdi-magnify"></v-btn>
    </v-app-bar>

    <Sidebar :drawer="drawer" />
</template>

<script setup>
import Sidebar from './sidebar.vue';
import { ref } from 'vue'

const drawer = ref(false);

</script>
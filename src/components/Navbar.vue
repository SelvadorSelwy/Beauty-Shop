<!-- eslint-disable vue/multi-word-component-names -->
<!-- eslint-disable prettier/prettier -->
<!-- eslint-disable vue/multi-word-component-names --><!-- eslint-disable prettier/prettier -->
<!-- eslint-disable vue/multi-word-component-names -->
<template>
    <v-app-bar app color="white" flat>
        <v-badge color="transparent" overlap content="" class="mr-2 mt-1">
            <v-img src="logo2.png" contain width="50"></v-img>
        </v-badge>
        <v-toolbar-title class="ml-4">
            <span class="eTitle">e</span><strong>Beauty</strong>
        </v-toolbar-title>
        <v-spacer></v-spacer>
        <v-badge color="#ff6d59" overlap content="2" class="mr-2 mt-1">
            <v-avatar color="#fffdee" size="40">
                <v-icon x-small color="ff6d59">far fa-heart</v-icon>
            </v-avatar>
        </v-badge>
        <v-badge color="#41AB55" overlap content="3" class="mr-2 mt-1">
            <v-avatar color="#ECF7EE" size="40">
                <v-icon x-small color="#41AB55">fas fa-shopping-cart</v-icon>
            </v-avatar>
        </v-badge>
        <span class="grey--text d-none d-sm-flex">Hello <strong> Selvador</strong></span>
        <v-avatar size="50" class="ml-2">
            <v-img src="SELWY2.jpg"></v-img>
        </v-avatar>
        <v-btn icon color="pink">
            <v-icon x-small>fas fa-chevron-down</v-icon>
        </v-btn>
    </v-app-bar>
</template>

<script>
export default {

}
</script>

<style></style>
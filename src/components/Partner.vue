<!-- eslint-disable vue/multi-word-component-names -->
<template>
    <v-row class="px-16 mt-10">
        <v-col cols="3" v-for="(partner, i) in partners" :key="i">
            <div align="center" justify="center">
                <v-img :src="partner.img" max-height="120" max-width="120" contain></v-img>
            </div>
        </v-col>
    </v-row>
</template>

<script>
export default {
    data: () => ({
        partners: [
            { img: "sleek.png" },
            { img: "soni.png" },
            { img: "loreal.png" },
            { img: "wella.png" },
        ]
    })
}
</script>

<style></style>
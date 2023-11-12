<!-- eslint-disable vue/multi-word-component-names -->
<template>
    <v-footer dark padless>
        <v-card flat tile class="black white--text py-12 px-5" width="100%">
            <v-row>
                <v-col cols="12" xs="12" sm="6" md="4" class="pa-16">
                    <v-toolbar color="transparent" flat>
                        <v-badge color="#D5F0DE" dot>
                            <v-img src="logo2.png" style="border-radius:50%" contain width="50"></v-img>
                        </v-badge>
                        <v-toolbar-title class="ml-4">
                            <span class="eTitle">e</span><strong>Beauty</strong>
                        </v-toolbar-title>
                    </v-toolbar>
                    <v-card-text class="pt-2">
                        <v-btn v-for="icon in icons" :key="icon" class="mx-1 white--text" icon fab outlined small>
                            <v-icon size="20">
                                {{ icon }}
                            </v-icon>
                        </v-btn>
                    </v-card-text>
                </v-col>
                <v-col cols="12" xs="12" sm="6" md="2">
                    <v-card-text class="white--text pt-0">
                        <h3>About</h3>
                    </v-card-text>
                    <v-card-text class="grey--text">How it work?</v-card-text>
                    <v-card-text class="grey--text mt-n4">Our Program</v-card-text>
                    <v-card-text class="grey--text mt-n4">Promotions</v-card-text>
                    <v-card-text class="grey--text mt-n4">Refer a Friend</v-card-text>
                </v-col>
                <v-col cols="12" xs="12" sm="6" md="2">
                    <v-card-text class="white--text pt-0">
                        <h3>Delivery</h3>
                    </v-card-text>
                    <v-card-text class="grey--text">Cost in Delivery</v-card-text>
                    <v-card-text class="grey--text mt-n4">Payment Method</v-card-text>
                    <v-card-text class="grey--text mt-n4">Delivery Astus</v-card-text>
                    <v-card-text class="grey--text mt-n4">Returns</v-card-text>
                </v-col>
                <v-col cols="12" xs="12" sm="6" md="4">
                    <v-card-text class="white--text pt-0">
                        <h3>Contact</h3>
                    </v-card-text>
                    <v-card-text class="grey--text">Selvador</v-card-text>
                    <v-card-text class="grey--text mt-n4">Hawban Road</v-card-text>
                    <v-card-text class="grey--text mt-n4">Selwy.com</v-card-text>
                    <v-card-text class="grey--text mt-n4">00967737081265</v-card-text>
                </v-col>
            </v-row>
        </v-card>
    </v-footer>
</template>

<script>
export default {
    data: () => ({
        icons: [
            "fab fa-apple",
            "fab fa-linkedin",
            "fab fa-twitter",
            "fab fa-telegram"
        ]
    })

}

</script>

<style></style>
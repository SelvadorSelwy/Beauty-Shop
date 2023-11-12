<!-- eslint-disable vue/multi-word-component-names -->
<template>
    <v-row justify="center" class="space px-16">
        <v-col cols="12" xs="12" sm="6" md="4" v-for="(product, i) in products " :key="i">
            <v-card class="mx-auto rounded-x1 borderme trans" max-width="250" outlined>
                <div align="center" justify="center">
                    <v-img max-height="190" max-width="250" contain :src="product.img"></v-img>
                </div>
                <v-card-title class="title1">{{ product.title }}</v-card-title>
                <v-card-title class="grey--text text-grey-darken-1 caption mt-n6">{{ product.subtitle }}</v-card-title>
                <v-card-title class="mt-n4">{{ product.price }}</v-card-title>
                <v-card-actions class="mx-2 mt-n4">
                    <v-btn outlined class="mt-n2 add">
                        <v-icon color="pink" @click="decrement">fas fa-minus</v-icon>
                    </v-btn>
                    <strong class="mx-2" v-text="quantity"></strong>
                    <v-btn outlined class="mt-n2 add">
                        <v-icon color="pink" @click="increment">fas fa-plus</v-icon>
                    </v-btn>
                    <v-spacer></v-spacer>
                    <v-btn class="mx-2 mt-n3" fab dark small color="pink">
                        <v-icon dark>fa-shopping-bag</v-icon>
                    </v-btn>
                </v-card-actions>
            </v-card>
        </v-col>
    </v-row>
</template>

<script>
export default {
    data: () => ({
        quantity: 1,
        products: [
            { img: "products/p (1).jpg", title: "Vaseline", subtitle: "100g", price: "5 SR" },
            { img: "products/p (2).jpg", title: "Nail paint", subtitle: "Golden", price: "3 SR" },
            { img: "products/p (3).jpg", title: "Nail Paint", subtitle: "Selver", price: "3 SR" },
            { img: "products/p (4).jpg", title: "Nail Paint", subtitle: "Dark Green", price: "3 SR" },
            { img: "products/p (5).jpg", title: "Lip Fresher", subtitle: "Strawperry", price: "2 SR" },
            { img: "products/p (6).jpg", title: "Nail Paint", subtitle: "Brown", price: "3 SR" },
            { img: "products/p (7).jpg", title: "Paint Pen", subtitle: "100g", price: "5 SR" },
            { img: "products/p (8).jpg", title: "Thick Pen", subtitle: "yellow", price: "3 SR" },
            { img: "products/p (9).jpg", title: "Perfuem", subtitle: "Love", price: "3 SR" },
            { img: "products/p (10).jpg", title: "Perfuem", subtitle: "Rose", price: "3 SR" },
            { img: "products/p (11).jpg", title: "Maskara", subtitle: "Black", price: "2 SR" },
            { img: "products/p (12).jpg", title: "Nail Paint", subtitle: "Golden", price: "3 SR" },
        ]
    }),
    methods: {
        decrement() {
            this.quantity--;
        },
        increment() {
            this.quantity++;
        }
    }
}
</script>

<style></style>
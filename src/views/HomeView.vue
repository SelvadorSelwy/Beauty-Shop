<template>
  <v-app>
    <Navbar />
    <v-container fluid class="me">
      <v-row>
        <v-col cols="12">
          <v-card class="mx-outo rounded xl" flat>
            <v-img src="w5.jpg" max-height="100%" max-width="100%" contain>
              <!-- ----- -->
              <v-card-text class="ml-10">
                <v-row>
                  <v-col cols="4">
                    <v-text-field label="Search you beauty source" class="d-none d-sm-flex d-md-flex" filled solo
                      prepend-inner-icon="md1-magnify" flat rounded success>
                    </v-text-field>
                  </v-col>
                  <v-col cols="2" class="marginLeft">
                    <v-btn color="var(--firstCo)" rounded dark class="py-7 d-none d-sm-flex d-md-flex">
                      Search
                    </v-btn>
                  </v-col>
                </v-row>
              </v-card-text>
              <v-card-title class="top ml-10">
                <h2 class="title1">High Quality</h2>
              </v-card-title>
              <v-card-title class="ml-10 mt-n8">
                <h2 class="title1">Order NOw</h2>
              </v-card-title>
              <v-card-text class="ml-10">
                <h3 class="pink--text">Free Delevery</h3>
              </v-card-text>
            </v-img>
          </v-card>
          <v-toolbar flat color="transparent">
            <v-btn-toggler v-model="toggle_exclusive">
              <v-btn rounded color=var(--firstCo) dark>
                <v-icon>fas fa-chevron-left</v-icon>
              </v-btn>
            </v-btn-toggler>
            <v-spacer></v-spacer>
            <v-toolbar-title class="text-h6">Category</v-toolbar-title>
            <v-spacer></v-spacer>
            <v-btn-toggler v-model="toggle_exclusive">
              <v-btn rounded color=var(--firstCo) dark>
                <v-icon>fas fa-chevron-right</v-icon>
              </v-btn>
            </v-btn-toggler>
          </v-toolbar>
          <Category />
          <v-toolbar flat color="transparent" class="mt-5">
            <v-toolbar-title class="text-h6">Popular Product</v-toolbar-title>
            <v-spacer></v-spacer>
            <v-btn rounded color="pink" dark class="ps-8">See All</v-btn>
          </v-toolbar>
          <Product />
          <v-card flat color="#E2F2E5" class="mt-8 py-5 px-16">
            <div style="position:absolute; margin-left: auto; margin-right:auto; left:0; right:0; text-align:center">
              <h3>What Our Clients Say?</h3>
            </div>
            <Client />
          </v-card>
          <v-toolbar flat color="transparent" class="mt-8">
            <v-toolbar-title class="text-h6">
              Our Sponsers
            </v-toolbar-title>
          </v-toolbar>
          <Partner />
          <v-card flat color="#E2F2E5" class="rounded-x1 mtop mbottom mx-10 pa-4" height="350">
            <v-row>
              <v-col cols="12" xs="12" sm="12" md="5">
                <v-card class="mt-n16 ml-16 mobile" rounded-x2 outlined flat height="450" width="200">
                  <v-img src="mobile1.png" contain style="margin-top:5px"></v-img>
                </v-card>
              </v-col>
              <v-col cols="12" xs="12" sm="6" md="7">
                <h1 class="mt-16">Download App</h1>
                <P>
                  Download our app into you mobile via google store or app store , <br />
                  inorder to be updated.pick you order from you mobile directely , <br />
                  you will be noticed emmidately after we
                  update our store.
                </P>
                <v-btn color="black" dark class="mt-4">
                  <v-icon color="white" left>fab fa-apple</v-icon>
                  App Store
                </v-btn>
                <v-btn color="black" dark class="ml-4 mt-4">
                  <v-icon color="white" left>fab fa-google-play</v-icon>
                  Play Store
                </v-btn>
              </v-col>
            </v-row>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
    <Footer />
  </v-app>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import Category from "@/components/Category.vue";
import Product from "@/components/Product.vue";
import Client from "@/components/Client.vue";
import Partner from "@/components/Partner.vue"
import Footer from "@/components/Footer.vue"

export default {
  name: "Home-page",
  data: () => ({
    toggle_exclusive: 1,
  }),
  components: {
    Navbar,
    Category,
    Product,
    Client,
    Partner,
    Footer,
  },
};
</script>

<style>
.me {
  background-color: #fff;
}

.v-card.trans {
  background-color: transparent;
}

.marginLeft {
  margin-left: -90px;
}

.mtop {
  margin-top: 100px;
}

.top {
  margin-top: 10px;
}

.mbottom {
  margin-bottom: 100px;
}

.v-card.borderme {
  border: 1px solid var(--secondCo) !important;
}

.v-card.borderout {
  border: 1px solid var(--firstCo) !important;
}

.v-btn:not(.v-btn-round).v-size--default.add {
  min-width: 0px !important;
}

.theme--light.v-sheet--outlined.mobile {
  border: 2px solid rgb(153, 50, 50) !important;
  border-radius: 20px !important;
}

.title1 {
  color: var(--firstCo);
}

@media only screen and (max-width:600px) {
  h2.title1 {
    font-size: 15px;
    color: var(--firstCo);
    margin-top: 10px;
  }

  h2.title2 {
    font-size: 15px !important;
    margin-top: 10px;
  }

  .top {
    margin-top: 10px !important;
  }
}

@media only screen and (min-width: 600px) {
  .top {
    margin-top: 30px;
  }
}

@media only screen and (min-width: 760px) {
  .top {
    margin-top: 50px !important;
  }
}
</style>
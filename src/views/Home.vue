<template>
  <div class="home">
    <section>
      <v-parallax :src="images.parallax" height="650">
        <v-container>
          <v-row column>
            <v-col
              class="text-md-center text-xl-center text-md-center text-lg-center"
            >
              <div class="display-2 font-weight-thin">
                ASTRONOMY
                <span class="white--text font-weight-light ">CLUB</span>
              </div>
              <div class="font-weight-light">
                Somewhere, something incredible is waiting to be known
              </div>
              <div class="mt-5">
                <v-btn outlined color="white">Learn More</v-btn>
              </div>
            </v-col>
          </v-row>
        </v-container>
      </v-parallax>
    </section>
    <section>
      <v-container>
        <v-row>
          <v-col
            class="my-12"
            v-for="(item, i) in items"
            :key="i"
            cols="12"
            md="12"
            sm="12"
          >
            <v-card dark>
              <v-container>
                <v-card-title class="display-1 font-weight-thin text-uppercase">
                  {{ item.title }}
                </v-card-title>
                <div>
                  <v-img :src="item.image" max-width="400"></v-img>
                </div>
              </v-container>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </section>
  </div>
</template>

<script>
// @ is an alias to /src
import parallax from "../assets/parallax5.jpg";
import bio from "../assets/bio.jpg";
import bh from "../assets/bh.jpg";
import phy from "../assets/phy.jpg";
import stars from "../assets/stars.jpg";
export default {
  name: "Home",
  components: {},
  data: () => ({
    images: {
      parallax
    },
    items: [
      { title: "Astro Biology", content: "", image: bio },
      { title: "Astro Physic", content: "", image: phy },
      { title: "Black hole", content: "", image: bh },
      { title: "Stars", content: "", image: stars }
    ]
  })
};
</script>

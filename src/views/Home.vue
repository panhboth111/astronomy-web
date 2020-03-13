<template>
  <div class="home">
    <section>
      <v-parallax :src="images.test2" height="650">
        <v-container>
          <v-row column>
            <v-col
              class="text-md-center text-xl-center text-md-center text-lg-center "
            >
              <div class="display-2 font-weight-thin">
                ASTRONOMY
                <span class="white--text font-weight-light ">CLUB</span>
              </div>
              <div class="font-weight-light">
                Somewhere, something incredible is waiting to be known
              </div>
              <div class="mt-5">
                <v-btn outlined color="white">read More</v-btn>
              </div>
            </v-col>
          </v-row>
        </v-container>
      </v-parallax>
    </section>
    <section class="my-md-10">
      <v-card color="transparent">
        <v-container>
          <v-card-title
            class="headline font-weight-thin justify-center white--text text-uppercase"
          >
            What is astronomy ?
          </v-card-title>
          <v-row>
            <v-col sm="12" md="6" cols="12">
              <v-img :src="images.pic3" max-width="600px"> </v-img>
            </v-col>
            <v-col sm="12" md="6" cols="12">
              <v-card-content class="white--text title font-weight-thin">
                Astronomy is the study of the sun, moon, stars, planets, comets,
                gas, galaxies, gas, dust and other non-Earthly bodies and
                phenomena. In curriculum for K-4 students, NASA defines
                astronomy as simple "the study of stars, planets and space."
                Astronomy and astrology were historically associated, but
                astrology is not a science and is no longer recognized as having
                anything to do with astronomy. Below we discuss the history of
                astronomy and related fields of study, including cosmology.
              </v-card-content>
            </v-col>
          </v-row>
        </v-container>
      </v-card>
    </section>
    <section class="mt-10">
      <v-parallax :src="images.test5" height="500" class="bg">
        <v-container>
          <v-row column>
            <v-col
              class="text-md-center text-xl-center text-md-center text-lg-center"
            >
              <div class="font-weight-light">
                There are many branches of astronomy
              </div>
              <div class="mt-5">
                <v-btn color="orange" outlined>EXPLORE</v-btn>
              </div>
            </v-col>
          </v-row>
        </v-container></v-parallax
      >
    </section>
    <footer class="mt-12">
      <v-container>
        <v-row>
          <v-col
            class="text-center white--text headline font-weight-thin"
            md="6"
            sm="12"
            cols="12"
          >
            Other astronomy-related sites
          </v-col>
          <v-col
            class="text-center white--text title font-weight-thin"
            md="6"
            sm="12"
            cols="12"
          >
            <div>timeanddate.com</div>
            <div>space.com</div>
            <div>earthsky.org</div>
            <div>nasaspaceflight.com</div>
            <div>zeiss.com</div>
            <div>moongiant.com</div>
          </v-col>
        </v-row>
      </v-container>
    </footer>
  </div>
</template>

<script>
// @ is an alias to /src
import parallax from "../assets/parallax5.jpg";

import pic3 from "../assets/test.jpg";
import test2 from "../assets/test2.jpg";
import test5 from "../assets/test5.jpg";

export default {
  name: "Home",
  components: {},
  data: () => ({
    images: {
      parallax,
      pic3,
      test2,
      test5
    }
  })
};
</script>
<style scoped></style>

<template>
  <div>
    <laptop />
    <link
      rel="stylesheet"
      href="https://fonts.googleapis.com/css?family=Sofia"
    />
    <video
      width="100%"
      class="blurry-load mb-8"
      autoplay
      loop
      muted
      id="video"
      playsinline
      preload="none"
    >
      <source src="../assets/technology.mp4" type="video/mp4" />
    </video>
    <v-container style="margin-top: 120px">
      <v-layout class="d-flex justify-space-between" row wrap>
        <v-flex sm5 xs12>
          <div class="name">
            <h1>How we stand out-We are Proactive Experts.</h1>
            <p>
              We Proactively consult, design, develop & scale robust web, mobile
              & custom software solutions, that fuel innovation & deliver
              digital success.
            </p>
            <p>
              At Futuris Tech we believe that every project is an important
              milestone in our journey. So we position ourselves as a boutique
              digital agency, custom tailoring impactful digital solutions with
              industry best practices across the board, for Fortune 500's, SMEs,
              and Start-up’s around the globe.
            </p>
          </div>
        </v-flex>
        <v-flex sm6 class="users">
          <v-img src="../assets/download.jpg"></v-img>
        </v-flex> </v-layout
    ></v-container>
    <div class="core" style="margin-top: 100px">
      <h1 class="text-h3 font-weight-bold d-flex justify-center">
        CORE SERVICES
      </h1>
    </div>
    <v-card height="460px" elevation="5">
      <v-carousel height="460px" cycle show-arrows-on-hover hide-delimiters>
        <v-carousel-item
          v-for="(item, i) in itemse"
          :key="i"
          :title="item.title"
          transition="fade-transition"
        >
          <v-layout row wrap justify-space-around>
            <v-flex md6 xs12>
              <v-img
                width="100%"
                height="450px"
                class="mt-4"
                :src="item.src"
              ></v-img> </v-flex
            ><v-flex class="hidden-sm-and-down" md5
              ><v-card-title class="ml-6">
                <span class="text-h4 mt-4" style="color: rgb(6, 177, 219)">
                  {{ item.title }}
                </span>
              </v-card-title>
              <v-card-text class="text-h6 ml-6 mr-16 pr-16">
                {{ item.text }}
              </v-card-text>
              <v-card-actions>
                <v-btn
                  class="ml-10 mt-12 underli"
                  style="text-decoration: none"
                  outlined
                  :to="item.route"
                >
                  View more
                </v-btn>
              </v-card-actions>
            </v-flex>
            <v-flex md1> </v-flex>
          </v-layout>
        </v-carousel-item>
      </v-carousel>
    </v-card>
    <v-layout row wrap>
      <v-flex class="d-flex justify-center" md12>
        <v-btn
          to="/contact-us"
          style="text-decoration: none"
          class="button"
          large
          >Contact us</v-btn
        >
      </v-flex>
    </v-layout>
    <div class="core" style="margin-top: 100px">
      <h1 class="text-h3 font-weight-bold d-flex justify-center">
        CORE SERVICES
      </h1>
    </div>
    <v-main>
      <v-layout row wrap class="mt-16 pt-12">
        <v-flex xs12 md12 class="testing white--text">
          <h1 class="text-h3 ml-4 font-weight-bold d-flex justify-center">
            Portfolio that speak!
          </h1>
        </v-flex>
      </v-layout>
    </v-main>
    <v-main>
      <v-layout row wrap class="mt-16 pt-8">
        <v-flex md5 xs9>
          <v-img
            width="600px"
            class="ml-12"
            src="../assets/mubail.jpeg"
          ></v-img>
        </v-flex>
        <v-flex md5 xs11>
          <h1 class="name">An award-winning video streaming app platform</h1>
          <p class="mt-8 ml-16">
            We designed and developed this AI powered video streaming platform
            to give a tiff to streaming giants like Netflix and Hulu. We created
            an out of the box experience to help make the product award-winning.
          </p>
          <v-btn
            outlined
            large
            to="/work/portfolio"
            class="underli ml-16 mb-12"
            style="margin-top: 100px; text-decoration: none"
            >View Portfolio</v-btn
          >
        </v-flex>
      </v-layout>
    </v-main>
    <v-main>
      <v-layout row wrap>
        <v-flex xs12 md12 class="d-flex justify-center">
          <h1 class="font-weight-bold black--text text-h3 mt-16 pt-16">
            Our process
          </h1>
        </v-flex>
      </v-layout>
      <div class="mt-8">
        <v-layout wrap row>
          <v-flex xs12 md6>
            <v-img
              height="500px"
              width="750px"
              src="../assets/zain.jpg"
            ></v-img>
          </v-flex>
          <v-flex md5 xs12 cols="4" class="ml-8">
            <h2 class="name">DISCOVERY WORKSHOP</h2>
            <p>
              We give the utmost importance to understand and document client’s
              inputs, design, and branding preferences. And clarify all the
              open-ended points to establish a precise and clear idea about both
              clients’ and project’s goals. We work in a collaborative approach
              involving key stakeholders to bring alignment in the business
              process.
            </p>
            <v-btn
            class="body"
              >Get in touch</v-btn
            >
          </v-flex>
        </v-layout>
      </div>
    </v-main>
  </div>
</template>
<script>
import laptop from "./laptop.vue";
export default {
  name: "main",
  components: {
    laptop,
  },
};
</script>

<style>
.users {
  border: 1px solid #ddd;
  border-radius: 4px;
  padding: 5px;
  width: 600px;
  height: 350px;
}
.name {
  font-family: "Sofia", sans-serif;
}
.core {
  background: rgb(8, 75, 87);
  background: linear-gradient(
    90deg,
    rgba(6, 43, 49, 0.939) 14%,
    rgb(62, 165, 184) 81%,
    rgba(122, 162, 202, 0.664) 100%
  );
}
/* From cssbuttons.io */
button {
  --glow-color: rgb(217, 176, 255);
  --glow-spread-color: rgba(191, 123, 255, 0.781);
  --enhanced-glow-color: rgb(231, 206, 255);
  --btn-color: rgb(100, 61, 136);
  border: 0.25em solid var(--glow-color);
  padding: 1em 3em;
  color: var(--glow-color);
  font-size: 15px;
  font-weight: bold;
  background-color: var(--btn-color);
  border-radius: 1em;
  outline: none;
  box-shadow: 0 0 1em 0.25em var(--glow-color),
    0 0 4em 1em var(--glow-spread-color),
    inset 0 0 0.75em 0.25em var(--glow-color);
  text-shadow: 0 0 0.5em var(--glow-color);
  position: relative;
  transition: all 0.3s;
}

button::after {
  pointer-events: none;
  content: "";
  position: absolute;
  top: 120%;
  left: 0;
  height: 100%;
  width: 100%;
  background-color: var(--glow-spread-color);
  filter: blur(2em);
  opacity: 0.7;
  transform: perspective(1.5em) rotateX(35deg) scale(1, 0.6);
}

button:hover {
  color: var(--btn-color);
  background-color: var(--glow-color);
  box-shadow: 0 0 1em 0.25em var(--glow-color),
    0 0 4em 2em var(--glow-spread-color),
    inset 0 0 0.75em 0.25em var(--glow-color);
}

button:active {
  box-shadow: 0 0 0.6em 0.25em var(--glow-color),
    0 0 2.5em 2em var(--glow-spread-color),
    inset 0 0 0.5em 0.25em var(--glow-color);
}
.body {
  appearance: none;
  background-color: #FFFFFF;
  border-radius: 40em;
  border-style: none;
  box-shadow: #ADCFFF 0 -12px 6px inset;
  box-sizing: border-box;
  color: #000000;
  cursor: pointer;
  display: inline-block;
  font-family: -apple-system,sans-serif;
  font-size: 1.2rem;
  font-weight: 700;
  letter-spacing: -.24px;
  margin: 0;
  outline: none;
  padding: 1rem 1.3rem;
  quotes: auto;
  text-align: center;
  text-decoration: none;
  transition: all .15s;
  user-select: none;
  -webkit-user-select: none;
  touch-action: manipulation;
}

.button-73:hover {
  background-color: #FFC229;
  box-shadow: #FF6314 0 -6px 8px inset;
  transform: scale(1.125);
}

.button-73:active {
  transform: scale(1.025);
}

@media (min-width: 768px) {
  .button-73 {
    font-size: 1.5rem;
    padding: .75rem 2rem;
  }
}
</style>
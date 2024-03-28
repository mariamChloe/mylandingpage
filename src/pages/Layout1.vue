<template>
  <q-page>
    <div class="row">
      <q-parallax src="building.jpg">
        <Typewriter title="We help makers " :words="adjs"> </Typewriter>
        <q-icon color="white" name="fas fa-chevron-down"></q-icon>
        <q-icon color="white" name="fas fa-chevron-down"></q-icon>
        <q-btn to="#news" class="q-mt-md" color="primary">Sign Up Now</q-btn>
      </q-parallax>
    </div>
    <Section img="code.jpg" />
    <Features :data="features" />
    <a id="news" />
    <Newsletter />
  </q-page>
</template>

<script>
import Typewriter from "../components/Typewriter";
import Section from "../components/Section";
import Features from "../components/Features";
import Newsletter from "../components/Newsletter";

export default {
  data() {
    return {
      adjs: ["create", "develop", "design"],
      features: [
        {
          title: "Developpement web",
          icon: "fas fa-rocket",
          text:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Veniam cupiditate ex earum soluta accusantium id corrupti sit deserunt dolorem ut, eius, numquam illo perferendis, reiciendis tempore quis at libero laudantium?"
        },
        {
          title: "DevOps",
          icon: "fas fa-rocket",
          text:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Veniam cupiditate ex earum soluta accusantium id corrupti sit deserunt dolorem ut, eius, numquam illo perferendis, reiciendis tempore quis at libero laudantium?"
        },
        {
          title: "Cybersecurity",
          icon: "fas fa-rocket",
          text:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Veniam cupiditate ex earum soluta accusantium id corrupti sit deserunt dolorem ut, eius, numquam illo perferendis, reiciendis tempore quis at libero laudantium?"
        }
      ]
    };
  },
  components: {
    Typewriter,
    Section,
    Features,
    Newsletter
  }
};
</script>

<style scoped>
.q-icon {
  font-size: 3em;
}
</style>

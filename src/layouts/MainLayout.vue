<template>
  <q-layout view="lHh Lpr lff">
    <q-header dark class="bg-green">
      <q-toolbar>
        <q-avatar>
        </q-avatar>
        <q-toolbar-title>
          Home
        </q-toolbar-title>
        <q-space />
        <q-btn flat to="/layout1">Contact</q-btn>
        <q-btn flat to="/layout2">a propos</q-btn>
        <q-btn flat to="/layout1">Nos services</q-btn>

      </q-toolbar>
    </q-header>
    <q-page-container>
      <router-view />
    </q-page-container>
    <Footer />
  </q-layout>
</template>

<script>
import Footer from "../components/Footer";

export default {
  name: "MainLayout",
  data() {
    return {
      leftDrawerOpen: false
    };
  },
  components: {
    Footer
  }
};
</script>

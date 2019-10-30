<template>
  <Router :routes="routes"></Router>
</template>

<script>
import Router from './Router.vue';

import HomePage from './HomePage.vue';
import AboutPage from './AboutPage.vue';
import BlogPage from './BlogPage.vue';
import ContactPage from './ContactPage.vue';
import NotFoundPage from './NotFoundPage.vue';
import PictureFirstPageVue from './PictureFirstPage.vue';
import Picture2PageVue from './Picture2Page.vue';
import Picture3PageVue from './Picture3Page.vue';

export default {
  data: () => ({
    routes: {
      default: NotFoundPage,
      '/': HomePage,
      '/about': AboutPage,
      '/blog': BlogPage,
      '/contacts': ContactPage,
      '/picture1': PictureFirstPageVue,
      '/picture2': Picture2PageVue,
      '/picture3': Picture3PageVue,
    }
  }),

  components: { Router }
}
</script>
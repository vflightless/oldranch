<template>
  <b-container  align-v="center" fluid>
    <b-row style="height:100vh;" align-v="center">
      <b-container class="mx-auto text-center bg-dark rounded text-white">
        <h1>Old Ranch</h1>
        <h6>Pull up...</h6>
        <b-nav fill align="center">
          <b-nav-item><NuxtLink to="/about">About</NuxtLink></b-nav-item>
          <b-nav-item><NuxtLink to="/blog">Blog</NuxtLink></b-nav-item>
        </b-nav>
      </b-container>
      
    </b-row>
  </b-container>
</template>

<script>
import client from '~/plugins/contentful';
import Navbar from '~/components/navbar.vue';
import bgUrl from '~/assets/chbg-upscale.png';

export default {
    asyncData() {
        return client.getEntries({
            content_type: "post",
        })
            .then(entries => {
            return { posts: entries.items };
        })
            .catch(e => console.log(e));
    },
    layout: 'home',
    data() { return { bgUrl } },
}
</script>

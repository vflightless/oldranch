<template>
  <section>
    <b-container class="mx-auto text-center" fluid>
      <h1>Old Ranch</h1>
      <h6>Pull up...</h6>
    </b-container>
  </section>
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
    components: { Navbar },
    layout: 'home',
    data() { return { bgUrl } },
}
</script>

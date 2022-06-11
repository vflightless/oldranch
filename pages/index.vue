<template>
  <b-row align-v="center" class="h-100" fluid>
    <b-col class="mx-auto text-center rounded text-dark">
        <h1>Pull up...</h1>
    </b-col>
  </b-row>
</template>

<script>
import client from '~/plugins/contentful';
import Navbar from '~/components/navbar.vue';

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
}
</script>
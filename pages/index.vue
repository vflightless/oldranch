<template>
  <section>
    <Navbar />
    <div>
      <h1>Old Ranch</h1>
      <h6>Pull up...</h6>
    </div>
  </section>
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
    components: { Navbar }
}
</script>

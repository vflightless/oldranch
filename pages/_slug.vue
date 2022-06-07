<template>
  <section>
      <Navbar /> 
    <h1>{{ post.fields.title }}</h1>
    <div v-html="$md.render(post.fields.content)"></div>
  </section>
</template>

<script>
import client from '~/plugins/contentful';
import Navbar from '~/components/navbar.vue';

export default {
    asyncData({ params }) {
        return client.getEntries({
            content_type: "post",
            "fields.slug": params.slug,
        })
            .then(entries => {
            return { post: entries.items[0] };
        })
            .catch(e => console.log(e));
    },
    components: { Navbar }
}
</script>

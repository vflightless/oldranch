<template>
    <section>
        <Navbar />
        Blog
        <div>
            <h4>Latest Posts</h4>
            <hr />
            <div v-for="(post, index) in posts" :key="index">
            <NuxtLink :to="post.fields.slug">≈{{ post.fields.title }}</NuxtLink>
            </div>
        </div>
    </section>
</template>

<script>
import client from '~/plugins/contentful';

export default ({
    asyncData( params ) {
        return client.getEntries({
            content_type: 'post'
        }).then(entries => {
            return { posts: entries.items}
        }).catch(e => console.log(e))
    }
})
</script>

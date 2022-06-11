<template>
    <section>
        <b-navbar>
            <b-navbar-brand>
                <NuxtLink to="/"><h4>Old Ranch</h4></NuxtLink>
            </b-navbar-brand>
            <b-navbar-nav class="mx-auto" pills>
                <b-nav fill align="center">
                <b-nav-item><NuxtLink to="/about">About</NuxtLink></b-nav-item>
                <b-nav-item><NuxtLink to="/blog">Blog</NuxtLink></b-nav-item>
                </b-nav>
            </b-navbar-nav>
        </b-navbar>
        <hr />
    </section>
</template>

<script>
export default {
    
}
</script>
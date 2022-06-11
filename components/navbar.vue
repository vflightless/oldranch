<template>
    <section>
        <b-navbar id="navbg" class="d-inline-flex flex-md-column pb-0" fluid="md">
            <b-navbar-brand>
                <NuxtLink to="/"><h4 class=" px-1">Old Ranch</h4></NuxtLink>
            </b-navbar-brand>
            <b-nav-text>Get comfy <img style="max-width: 32px" src="~/assets/comfy.jpg" /></b-nav-text>
            <b-navbar-nav class="ml-auto mr-2" pills>
                    <b-nav-item><NuxtLink class="mx-3" to="/about" >About</NuxtLink></b-nav-item>
                    <b-nav-item><NuxtLink class="mx-3" to="/blog" >Blog</NuxtLink></b-nav-item>
            </b-navbar-nav>
            <!--<b-collapse id="navbar-toggle-collapse" is-nav>
                <b-navbar-nav class="ml-auto">
                    <b-nav-item><NuxtLink class="mx-3" to="/about" >About</NuxtLink></b-nav-item>
                    <b-nav-item><NuxtLink class="mx-3" to="/blog" >Blog</NuxtLink></b-nav-item>
                </b-navbar-nav>
            </b-collapse>-->
        </b-navbar>
        <hr class="my-0" />
    </section>
</template>

<script>
export default {
    
}
</script>

<style>
    #navbg {
        background-color: hsla(0, 0%, 100%, 0.7);
    }
</style>





<template>
<section class="my-0 bg-menu">
    <!-- Regular Menu -->
    <b-navbar toggleable="md" type="light" class="navbg">
        <b-navbar-brand><NuxtLink to="/">Old Ranch</NuxtLink></b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse class="mx-0 w-100" is-nav>
            <b-navbar-nav class="mx-0">
                <b-nav-text class="text-dark">Get comfy <img style="max-width: 32px;" src="~/assets/comfy.jpg"></b-nav-text>
            </b-navbar-nav>
            <b-navbar-nav class="ml-auto">
                <b-nav-item><NuxtLink class="mx-3" to="/about" >About</NuxtLink></b-nav-item>
                <b-nav-item><NuxtLink class="mx-3" to="/blog" >Blog</NuxtLink></b-nav-item>
            </b-navbar-nav>
        </b-collapse>
    </b-navbar>

    <!-- Collapse Menu -->
    <b-collapse id="nav-collapse" class="bg-dark" is-nav>
        <b-navbar-nav class="text-center">
            <b-nav-text class="text-light">Get comfy <img style="max-width: 32px;" src="~/assets/comfy.jpg"></b-nav-text>
            <b-nav-item><NuxtLink class="mx-3 text-light" to="/about" >About</NuxtLink></b-nav-item>
            <b-nav-item><NuxtLink class="mx-3 text-light" to="/blog" >Blog</NuxtLink></b-nav-item>
        </b-navbar-nav>
    </b-collapse>

    <hr class="my-0">
</section>
</template>

<script>
export default {
    
}
</script>
 <style scoped>
    .navbg {
        background-color: rgba(255, 255, 255, 0.904);
    }
 </style>
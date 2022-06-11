<template> 
    <section id="body-bg">
        <Navbar />
        <b-container style="height: 90vh;" fluid>
            <Nuxt />
        </b-container>
    </section>
</template>

<script>
import Navbar from '~/components/navbar.vue';

export default {
    layout: 'home',
    components: { Navbar },
}
</script>

<style scope>
  #body-bg {
    height: 100vh;

    background-image: url(~/assets/chbg-upscale.png);
    background-color: #bdfdfc;
    background-size: auto 100%;
    background-position: center right;
    background-repeat: no-repeat;
  }
</style>
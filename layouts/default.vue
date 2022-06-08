<template class="h-100">
    <section class="d-block h-100 w-100" :style="{ backgroundImage: `url(${bgImage})`}" style="background-size: cover;" >
        <b-container class="d-inline-block h-100">Get Fuqed</b-container>
        <h1>Default</h1>
        <Nuxt />
    </section>
</template>

<script>
import bgImg from "~/assets/chbg-upscale.png";

export default {
    layout: 'default',
    data() {
        return { bgImage: bgImg }
    }
}
</script>

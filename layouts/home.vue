<template>
    <section style="width: 100vw; height: 100vh; background-repeat: no-repeat; background-size: cover; background-position: right;" :style="{ backgroundImage: `url(${bgUrl})` }">
        <Nuxt />
    </section>
</template>

<script>
import bgUrl from '~/assets/chbg-upscale.png';

export default {
    layout: 'home',
    data() { return { bgUrl } },
}
</script>
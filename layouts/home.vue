<template> 
    <section>
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
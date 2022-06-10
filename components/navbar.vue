<template>
    <section>
        <b-navbar>
            <b-navbar-brand>
                <NuxtLink to="/"><h4>Old Ranch</h4></NuxtLink>
            </b-navbar-brand>
            <b-navbar-nav class="mx-auto" pills>
                <b-nav fill align="center">
                <NuxtLink to="/about"><b-nav-item>About</b-nav-item></NuxtLink>
                <NuxtLink to="/blog"><b-nav-item>Blog</b-nav-item></NuxtLink>
                </b-nav>
            </b-navbar-nav>
        </b-navbar>
        <hr />
    </section>
</template>
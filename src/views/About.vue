<template>
    <transition name="pageTransition">
        <section id="about">
            <h2 class="h2">About</h2>
            <div class="container-content">
                <p>I am based in Israel, in Jerusalem precisely. I make websites. I enjoy the constant discovering of new techniques, programming languages, frameworks, libraries, but also design trends and tools.</p>
                <p>The current website was made using the following concepts and technologies: PWA, VueJS, SPA, Firebase, Webpack, SVG, Sass, CSS animations, flat design, CSS grid. It was made with a will of being as minimalist as possible and keep the main information in front.</p>
                <p>I invite you to <router-link to="/">have a look at my work and the people I worked for</router-link>. Convinced? Need a cool website? <router-link to="/contact">Contact me</router-link> =)</p>
            </div>
        </section>
    </transition>
</template>

<script>
    export default {
      name: 'About'
    }
</script>

<template>
    <transition name="pageTransition">
      <section id="home">
        <h2 class="h2">Home</h2>
        <div class="container-content">
            <p>Welcome to LightWolf Studios, creation of web apps. I am Benjamin Meir Khalifa, and I hope you will enjoy my portfolio. I am here to design and develop websites with the latest design trends and technologies.</p>
            <p><router-link to="/projects">Check out my projects</router-link> and <router-link to="/contact">don't hesitate to contact me</router-link> afterwards =)</p>
            <p>You can also <router-link to="/about">learn more about LightWolf Studios and me</router-link> if you wish.</p>
        </div>
    </section>
</transition>
</template>

<script>
export default {
    name: 'Home'
}
</script>
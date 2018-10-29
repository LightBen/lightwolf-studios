<template>
    <header>
        <router-link to="/" title="LightWolf Studios">
            <div class="identity">
                <figure class="logo"></figure>
                <h1 class="h1">LightWolf Studios</h1>
            </div>
        </router-link>
        <div class="header-right">
            <figure class="night-icon" id="nightIcon"></figure>
            <figure class="menu-icon" id="menuIcon" @click="isClosed = !isClosed"></figure>
        </div>
        <div id="menu" class="menu" v-bind:class="{ closed : isClosed }">
            <div class="menu-item" @click="isClosed = !isClosed">
                <router-link to="/">Projects</router-link>
            </div>
            <div class="menu-item" @click="isClosed = !isClosed">
                <router-link to="/about">About</router-link>
            </div>
            <div class="menu-item" @click="isClosed = !isClosed">
                <router-link to="/contact">Contact</router-link>
            </div>
        </div>
    </header>
</template>

<script>
    import Menu from './Menu'

    export default {
        name: 'Header',
        // components: {
        //     'Menu': Menu
        // },
        data() {
            return {
                isClosed: true
            }
        }
    }
</script>
<template>
    <div id="menu" class="menu">
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
</template>

<script>
    export default {
        name: 'Menu',
        data() {
            return {
                isClosed: true
            }
        }
    }
</script>

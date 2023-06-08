<template>
        <div class="large-screen" v-if="!mobileView">
            <router-link to="/">Home</router-link> |
            <router-link to="/about">About</router-link> |
            <router-link to="/login">login</router-link> |
            <router-link to="/signup">signup</router-link> |
        </div>
        <div v-if="mobileView">
        <span class="main-span small-screen"  v-on:click="showNavMobile = !showNavMobile">
            <span></span>
            <span></span>
            <span></span>
        </span>

        <div class="mobile-nav" :class="{open : showNavMobile}">
            <router-link to="/">Home</router-link>
            <router-link to="/about">About</router-link>
            <router-link to="/login">login</router-link>
            <router-link to="/signup">signup</router-link>
        </div>
        </div>
    
    <!-- <router-view/> -->
</template>



<script>
export default {
    name: 'MobileNav',
    data() {
        return {
            mobileView: true,
            showNavMobile : false,
        }
    },
    methods:{
        mobileNavCheck () {
            this.mobileView = window.innerWidth <= 990;
        },
        convertClass(e) {
            console.log(e)
        }
    },
    created() {
        this.mobileNavCheck();
    },
}
</script>

<style>
nav a.router-link-exact-active {
    color: #42b983;
}
.mobile-nav {
    display: flex;
    position: fixed;
    background-color: #000;
    flex-direction: column;
    padding: 20px;
    gap: 20px;
    transform: translateX(100px);
    transition: .6s;
}
.open {
    transform: translateX(-100px);
}

.mobile-nav a {
    transition: .6s;
}

.mobile-nav a:hover {
    transform: scale(1.1);
}
</style>
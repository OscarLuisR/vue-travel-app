<template>
    <div id="app">
        <the-navigation />
        
        <router-view :key="$route.path" />
    </div>
</template>

<script>
    import TheNavigation from './components/TheNavigation.vue'

    export default {
        components: {
            TheNavigation
        }        
    }
</script>

<style>
    #app {
        font-family: Avenir, Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
    }

    .input {
        border: 1px solid green;
        padding: 10px;
        margin-bottom: 20px;
    }
    .btn {
        background-color: green;
        color: white;
        padding: 10px;
    }
    
</style>

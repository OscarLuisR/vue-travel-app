<template>
    <div>
        <span class="go-back">
            <button @click="goBack">Go Back</button>    
        </span>
    </div>
</template>

<script>
    export default {
        name: 'GoBack',
        methods: {
            goBack() {
                return this.$router.go(-1);
            }
        }
    }
</script>

<style scoped>
    .go-back {
        display: flex;
        cursor: pointer;
    }

    /* button {
        border: 0;
    } */
</style>
<template>
    <div class="v-main-wrapper">
        <v-catalog/>
        <v-cart/>
    </div>
</template>


<script> 

    import vCart from './v-cart.vue';
    import vCatalog from './v-catalog.vue';

    export default {
        name: "v-main-wrapper",
        components: {
            vCart,
            vCatalog,
        },
        
    } 
</script>


<style>

     .v-main-wrapper {
        max-width: 900px;
        margin: 0 auto;
    }

</style>
<template>
    <div class="v-catalog-item">
        <img :src="require('../assets/images/' + product_data.image)" alt="">
        <p>{{product_data.name}}</p>
        <p>{{product_data.price}}</p>
        <button @click="sendDataToParent">Add to cart</button>
    </div>
</template>

<script>

    export default {
        name: "v-catalog-item",
        data() {
          return {}
        },
        props: {
            product_data: {
                type: Object,
                default() {
                    return {}
                }
            }

        },

        methods: {
            sendDataToParent() {
                this.$emit('sendDataToParent', this.product_data.article)
            }
        }
    }

</script>


<style>

</style>

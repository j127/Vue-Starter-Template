<style>
    .red {
        color: #f00;
    }
</style>

<template>
    <div class="container">
        <h1>{{msg}}</h1>
        <jumbotron></jumbotron>
    </div>

</template>

<script>
import Jumbotron from './jumbotron.vue'
export default {
    data() {
        return {
            msg: 'Saluton, Mondo!'
        }
    },
    components: {
        Jumbotron
    }
}
</script>
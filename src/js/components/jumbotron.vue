<style scoped>
.jumbotron {
    margin-top: 9px;
}
</style>

<template>
    <div class="jumbotron">
        <h1>{{greeting}}</h1>
    </div>
</template>

<script>
export default {
    data() {
        return { greeting: 'Saluton, Mondo!' }
    },
    ready() {
        console.log('Saluta mesago de jumbotron.vue');
    },
}
</script>
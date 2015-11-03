<style scoped>
h1 {
    color: green;
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
        console.log('from jumbotron.vue');
    },
}
</script>
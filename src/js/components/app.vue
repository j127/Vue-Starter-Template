<style>

</style>

<template>
    <div class="container">
        <jumbotron></jumbotron>
        <div class="well">{{m}}</div>
        <ol>
            <li v-for="monster in monsters">{{monster.type | capitalize}}</li>
        </ol>
    </div>
    <pre><h3>Component Data</h3>{{ $data | json }}</pre>
</template>

<script>
import Jumbotron from './jumbotron.vue'
export default {
    data() {
        return {
            m: 'Mi ŝatas Vue-on.',
            monsters: [
                {'type': 'beholder'},
                {'type': 'kobold'},
                {'type': 'troll'},
                {'type': 'dragon'}
            ]
        }
    },
    ready() {
        console.log(this);
    },
    components: {
        Jumbotron
    }
}
</script>
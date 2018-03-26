<template>
    <div>
        <app-header></app-header>
        <app-main></app-main>
        <app-footer></app-footer>
    </div>
</template>

<script>
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
import HackerJobs from './components/HackerJobs.vue';

export default {
    components: {
        'app-header': Header,
        'app-footer': Footer,
        'app-main': HackerJobs
    },
    data () {
        return {
        }
    }
}

</script>

<style>
</style>

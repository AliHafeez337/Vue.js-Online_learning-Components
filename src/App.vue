<template>
    <div class="container">
        <app-header></app-header>
        <hr>
        <div class="row">
            <patients></patients>
        </div>
        <hr>
        <app-footer></app-footer>
    </div>
</template>

<script>
    import Header from './components/Shared/Header.vue';
    import Footer from './components/Shared/Footer.vue';
    import Patients from './components/Patients/Patients.vue';

    export default {
        components: {
            appHeader: Header,
            Patients,
            'app-footer': Footer
        }
    }
</script>

<style>

</style>

<template>
    <div class="col-xs-12 col-sm-6">
        <ul class="list-group">
            
            <app-patient-details
                class="list-group-item"
                v-for="(item, index) in 5"
                v-bind:key="index"
                ></app-patient-details>
        </ul>
    </div>
</template>

<script>
    import PatientsDetails from './PatientsDetails.vue';

    export default {
        components: {
            'app-patient-details': PatientsDetails
        }
    }
</script>

<style scoped>
    div {
        border: 1px solid blue;
        padding: 10px;
    }
</style>

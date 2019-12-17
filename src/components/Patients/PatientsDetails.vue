<template>
    <div class="col-xs-12 col-sm-6">
        <p>Patient status: {{ status }}</p>
        <hr />
        <button v-on:click="normalStatus()">Normal</button>
        <button v-on:click="criticalStatus()">Critical</button>
    </div>

</template>

<script>
    export default {
        data: function() {
            return {
                status: 'Critical'
            }
        },
        methods: {
            normalStatus() {
                this.status = 'Normal'
            },
            criticalStatus() {
                this.status = 'Critical'
            }
        },
        beforeUpdate() {
            console.log('before update')
        },
        updated() {
            console.log('updated')
        },
    }
</script>

<style scoped>
    div {
        border: 1px solid red;
    }
</style>

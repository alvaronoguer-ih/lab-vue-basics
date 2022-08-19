<template>
<div>
    <h1>Esto es un footer</h1>
    <h2> {{ myNumber }}</h2>
    <h3> {{ 3+3 }}</h3>
    <h3> {{ returnString() }} </h3>
    <h3> {{ project }}</h3>
</div>
</template>

<script>

export default {
    name: 'Footer', 
    props: {
        myNumber: Number,
    },

    data() {
        return {
            numb: 8,
            project: " ",
        }
    },

    methods: {
        returnString() {
            return "Hola Mundo";
        }
    },

    created() {
        this.project = 'Hola Mundo de nuevo';
    },
 
}


</script>

<style>

</style>
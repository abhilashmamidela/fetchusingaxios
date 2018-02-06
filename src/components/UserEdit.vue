<template>
    <div class="component">
        <h3>User details</h3>
        <p>User details are:{{myName.name}}</p>
        <p>{{myName.email}}</p>

        


    </div>
</template>

<script>
    export default{
        props:['myName']
    }
    
</script>

<style scoped>
    div {
        background-color: lightgreen;
    }
</style>

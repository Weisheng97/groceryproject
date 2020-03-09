<template>
    <div class = "headerStyle">
        <p1> Current Count: {{counter}} </p1>
        <br> <br>
        <button v-on:click="increment">+</button>
        <button v-on:click="decrement">-</button>
    </div>
</template>

<script>
export default {
    data() {
        return {
            counter: 0
        }
    },
    methods: {
        increment: function() {
            this.counter += 1;
            
        },
        decrement: function() {
            if(this.counter != 0) {
                this.counter -= 1;  
            }          
        }
    }
}
</script>

<style scoped>
header{
    background:rgb(122, 63, 100);
    padding:10px;
    border-style: solid;
    border-color:black;
    border-width: 2px;
}
h1{
    color:ivory
}
</style>
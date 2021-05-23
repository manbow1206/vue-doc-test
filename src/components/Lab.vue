<template>
    <div>
        <h1>{{ propData }}</h1>
        <p>{{ text }}</p>
    </div>
</template>

<script>
export default {
    props: ['propData'],
    data(){
        return {
            text: "Hello Vue.js!"
        }
    }
}
</script>

<style scoped>
div{
    border: 2px solid teal
}
h1{
    color: teal
}
p{
    color:rgb(27, 77, 77)
}
</style>

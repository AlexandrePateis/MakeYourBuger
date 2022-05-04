<template>
    <div class="main-banner">
        <h1>Make Your Burger</h1>
    </div>
</template>

<script>
export default {
    name:"Banner"    
}
</script>

<style scoped>
.main-banner{
    background-image: url('/public/img/burger.jpg');
    background-position: 0 -250px;
    background-size: cover;
    background-repeat: no-repeat;
    height: 900px;
    display: flex;
    align-items: center;
    justify-content: flex-start;
}
.main-banner h1{
    text-align: center;
    color: #FFF;
    font-size: 5em;
    padding: 1em;
    background-color: black;
    border-radius: 0.2em;
}
</style>
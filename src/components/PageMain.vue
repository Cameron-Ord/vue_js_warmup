<template>
    <div class="parent">
        <span class="main_span">

            <h1>Welcome to my E-commerse website!</h1>

            <p>I only sell the finest thunderfurys!</p>

        </span>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
.parent{

        display: grid;

        justify-items: center;

    align-items: center;

    text-align: center;
}

.parent>.main_span{

    background-color: #BEE3DB;
    
    display: grid;

    grid-template-rows: 15vh 15vh;

    justify-items: center;

align-items: center;

text-align: center;

padding-top: 75px;

padding-bottom: 75px;

width: 80%;
}
</style>
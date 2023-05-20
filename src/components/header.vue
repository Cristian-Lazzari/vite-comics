<script>
export default {
    data(){
        return{
            vociMenu:[
                'CHARACTCERS',
                'COMICS',
                'MOVIE',
                'GAMES',
                'COLLECTIBLES',
                'VIDEO',
                'FANS',
                'NEWS',
                'SHOP']
        }
    }
}
</script>
    
<template>
    <div class="container">
        <img src="../assets/img/dc-logo.png" alt="">
        <ul>
            <li v-for= "voce in vociMenu">{{ voce }}</li>
        </ul>
    </div>
 
</template>

<style lang="scss" scoped>
    .container{
        padding: 1rem;
        max-width: 990px;
        margin-inline: auto;
        background-color: white;
        color: black;
        display: flex;
        justify-content: space-between;
        align-items: center;
        gap: 1em;
        ul{
            display: flex;
            gap: 1em;
            
        }

    }
</style>
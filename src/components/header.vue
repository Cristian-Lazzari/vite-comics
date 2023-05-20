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
    <img src="../assets/img/dc-logo.png" alt="">
    <ul>
        <li v-for= "voce in vociMenu">{{ voce }}</li>
    </ul>
 
</template>

<style lang="sass">
    
</style>
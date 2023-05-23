<script>
export default {
    props: {
        img: String,
        title: String
    }

}
</script>
<template >
    <div class="container">
        <img :src="img" :alt="img">
        <h4>{{ title }}</h4>
    </div>
</template>
<style lang="scss" scoped>
    .container{
        color: white;
        max-width: calc(((100% - 4rem) - 1rem * 5 ) /4);
        img{
            width: 100%;
            object-fit: cover;
            aspect-ratio: 1;
            
        }
    }
</style>
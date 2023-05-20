<script>
import Aheader from './components/header.vue';
import Acontenent from './components/contenent.vue';
import Afooter from './components/footer.vue';


export default {
	components: {Aheader, Acontenent, Afooter }
};
</script>

<template>
  <div class="containet">
    <Aheader/>
    <Acontenent/>
    <Afooter/>

  </div>
	
</template>

<style lang="scss">
@use './assets/styles/general.scss' as *;
.container{
  
}

</style>

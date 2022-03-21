<template>
<div class="container row align-items-start">
   
        <div class="col-md-4 col-sm-4 col-12" :key="serie.id" v-for="serie in series">
            <Serie :serie="serie" />
        </div>
  
</div>
</template>

<script>
import Serie from './Serie.vue'

export default {
    name: 'Series',
    props: {
        series: Array,
    },
    components: {
        Serie
    },
    emits: [],
}
</script>


<style scoped>
.container {  
  margin: 30px auto;
  overflow: auto;
  min-height: 300px;
  /* border: 1px solid steelblue; */
  padding: 30px;
  border-radius: 5px;
}
</style>
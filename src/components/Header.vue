<template>
    <header>
        <div
      class="p-5 text-center bg-image"
      style="
        background-image: url('https://wallpapercave.com/wp/A9UHCmu.jpg');
        background-repeat: no-repeat;
        height: 400px;        
      "
    >
      <div class="mask" style="background-color: rgba(0, 0, 0, 0.6);">
        <div class="d-flex justify-content-center align-items-center h-100">
          <div class="text-white">
            <h1 class="mb-3">SIMON'S HAPPY PLACE</h1>
            <h4 class="mb-3">TV-SERIES</h4>            
          </div>
        </div>
      </div>     
    </div>
    </header>
</template>

<script>
import Button from './Button.vue'
import Navigation from './Navigation.vue'

export default({
    name: 'Header',
    props: {
        title: { type: String },
    },
    components: {
        Button,   
        }    
})
</script>

<style scoped>

</style>

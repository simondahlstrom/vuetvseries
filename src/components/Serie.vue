<template>
  <div class="card" style="margin-top:15px">
    <div class="card-body">
      <h5 class="card-title">
          {{ serie.title }} 
          <a :href="serie.url" target="_blank" class="card-link">
            <i class="fa-solid fa-link"></i>
          </a>
          <div class="card-class" style="">{{ serie.class }}</div>
      </h5>     
        <div class="genre-container">
          <section class="text-muted card-genre" :key="g" v-for="g in serie.genre">{{ g }}</section>
        </div>
        <div id="feeds" class="collapse">
          {{ serie.details }}
        </div>    
        {{ serie.details != undefined ? serie.details.length > 50 ? serie.details.substring(0,50)+"..." : serie.details : "" }}
        <a href="#feeds" data-toggle="collapse">Läs mer...</a>
    </div>
  </div>
</template>

<script>
var genreColors = [{'S':'green'},{'B':'blue'}];

export default {
    name: 'Serie',
    props: {
        serie: Object,
    },
    computed: {
      classObject: function () {
        return {
          active: this.isActive && !this.error,
        }
      }
    }
}
</script>

<style scope>
  .genre{
    word-spacing: 5px;
  }
  .genre-container{
    display: flex;
  }
  .card-title{
    font-size: 1.5em;
    font-weight: bold;
  }
  .card-genre{
    font-size: .9em;
  }
  .card-class{   
    font-size: .65em; 
    float:right;   
  }  
  .card-link > .fa-link{
    text-decoration: none;
    /* color: #000; */
    font-size: 0.6em;
  }
</style>

<template>
  <div class="">
    <Header title="Hello" />
    <Navigation />
    <Series :series="series" />
  </div>
</template>


<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import Header from './components/Header.vue';
import Series from './components/Series.vue';
import Navigation from './components/Navigation.vue';

@Options({
  components: {
    Header,
    Series,
    Navigation,
  },
  data(){
    return {
      series: []
    }
  },
  methods: {

  },
  created(){
    this.series = [
      {
        id: 1,
        title: 'Lucifer',
        url: 'https://www.rottentomatoes.com/tv/lucifer',
        class: 'Ⓢ',
        type: 'Series',
        genre: ['Crime','Drama','Fantasy'],
        details: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.',
      },
      {
        id: 2,
        title: 'Star Trek: Disovery',
        url: 'https://www.rottentomatoes.com/tv/star_trek_discovery',
        class: 'Ⓢ',
        type: 'Series',
        genre: ['Action','Adventure','Drama'],
        details: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.',
      },
      {
        id: 3,
        title: 'Supernatural',
        url: 'https://www.rottentomatoes.com/tv/supernatural',
        class: 'Ⓢ',
        type: 'Series',
        genre: ['Drama','Fantasy','Horror'],
        details: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.',
      },
      {
        id: 4,
        title: 'Doctor Who',
        url: 'https://www.rottentomatoes.com/tv/doctor_who',
        class: 'Ⓢ',
        type: 'Series',
        genre: ['Adventure','Drama','Sci-Fi'],
        details: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.',
      },
      {
        id: 5,
        title: 'Westworld',
        url: 'https://www.rottentomatoes.com/tv/westworld',
        class: 'Ⓢ',
        type: 'Series',
        genre: ['Drama','Mystery','Sci-Fi'],
        details: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.',
      },
      {
        id: 6,
        title: 'Black Sails',
        url: 'https://www.rottentomatoes.com/tv/black_sails',
        class: 'Ⓢ',
        type: 'Series',
        genre: ['Action','Adventure','Drama'],
        details: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.',
      },      
      {
        id: 7,
        title: 'Kingdom',
        url: 'https://www.rottentomatoes.com/m/kingdom',
        class: 'Ⓢ',
        type: 'Series',
        genre: ['Action','Drama','History'],
        details: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.',
      },
      {
        id: 8,
        title: 'Penny Dreadful',
        url: 'https://www.rottentomatoes.com/tv/penny-dreadful',
        class: 'Ⓑ',
        type: 'Series',
        genre: ['Drama','Fantasy','Horror'],
        details: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.',
      },      
      {
        id: 9,
        title: 'Frontier',
        url: 'https://www.rottentomatoes.com/tv/frontier',
        class: 'Ⓑ',
        type: 'Series',
        genre: ['Adventure','Drama','History'],
        details: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.',
      },   
      {
        id: 10,
        title: 'I Saw the Devil',
        url: 'https://www.rottentomatoes.com/m/akmareul_boattda',
        class: 'Ⓐ',
        type: 'Movie',
        genre: ['Action','Drama','Crime'],
        details: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.',
      },
      {
        id: 11,
        title: 'Killjoys',
        url: 'https://www.rottentomatoes.com/tv/killjoys',
        class: 'Ⓑ',
        type: 'Series',
        genre: ['Action','Adventure','Sci-Fi'],
        details: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.',
      },      
      {
        id: 12,
        title: 'Taboo',
        url: 'https://www.rottentomatoes.com/tv/taboo',
        class: 'Ⓐ',
        type: 'Series',
        genre: ['Drama','Mystry','Thriller'],
        details: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.',
      },
      {
        id: 13,
        title: 'Walker',
        url: 'https://www.rottentomatoes.com/tv/walker',
        class: '',
        type: 'Series',
        genre: ['Action','Crime','Drama'],
        details: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.',
      },
      {
        id: 14,
        title: 'The Irregulars',
        url: 'https://www.rottentomatoes.com/tv/the_irregulars',
        class: 'Ⓒ',
        type: 'Series',
        genre: ['Crime','Drama','Fantasy'],
        details: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.',
      },
      {
        id: 15,
        title: 'The Alienist',
        url: 'https://www.rottentomatoes.com/tv/the_alienist',
        class: 'Ⓑ',
        type: 'Series',
        genre: ['Crime','Drama','Mystery'],
        details: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.',
      },
      {
        id: 16,
        title: 'The Expanse',
        url: 'https://www.rottentomatoes.com/tv/the_expanse',
        class: 'Ⓑ',
        type: 'Series',
        genre: ['Drama','Mystery','Sci-Fi'],
        details: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.',
      },
      {
        id: 17,
        title: 'The Witcher',
        url: 'https://www.rottentomatoes.com/tv/the_witcher',
        class: 'Ⓐ',
        type: 'Series',
        genre: ['Action','Adventure','Drama'],
        details: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.',
      },
      {
        id: 18,
        title: 'Altered Carbon',
        url: 'https://www.rottentomatoes.com/tv/altered_carbon',
        class: 'Ⓑ',
        type: 'Series',
        genre: ['Action','Drama','Sci-Fi'],
        details: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.',
      },
      {
        id: 19,
        title: 'Torchwood',
        url: 'https://www.rottentomatoes.com/tv/torchwood',
        class: 'Ⓢ',
        type: 'Series',
        genre: ['Action','Drama','Mystery'],
        details: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.',
      }
    ];
  }
})
export default class App extends Vue {}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400&display=swap');
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body{
  font-family: 'Nunito', sans-serif;
}
.btn {
  display: inline-block;
  background: #000;
  color: #fff;
  border: none;
  padding: 10px 20px;
  margin: 5px;
  border-radius: 5px;
  cursor: pointer;
  text-decoration: none;
  font-size: 15px;
  font-family: inherit;
}
.btn:focus {
  outline: none;
}
.btn:active {
  transform: scale(0.98);
}
.btn-block {
  display: block;
  width: 100%;
}
</style>

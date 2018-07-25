<template>
  <div id="app">
    <div id="overlay"></div>
    <img class="bg-img" src="./assets/scott-webb-270034-unsplash.jpg" alt="person with backpack infront of bricks" height="100%" width="100%"></img>
    <Home/>
  </div>
</template>

<script>
import Home from './components/Home'
import CollegeList from './components/CollegeList'
import CollegeInfo from './components/CollegeInfo'

export default {
  name: 'App',
  components: {
    Home
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: silver;
}



app {
    height: 100%;
}

bg-img {
    /* Center and scale the image nicely */
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    margin: 0;
}

#overlay {
    position: fixed; /* Sit on top of the page content */
    width: 100%; /* Full width (cover the whole page) */
    height: 100%; /* Full height (cover the whole page) */
    top: 0; 
    left: 0;
    right: 0;
    bottom: 0;
    background-color: rgba(850,0,0,0.5); /* Black background with opacity */
    z-index: 2; /* Specify a stack order in case you're using a different order for other elements */
    cursor: pointer; /* Add a pointer on hover */
}
</style>

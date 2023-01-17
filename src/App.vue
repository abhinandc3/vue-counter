<template>
  <div id="app">
  <h1>vue events</h1>
  <h2>events in action</h2>
  <hr />
  <button @click="increment()">add</button>
  <button @click="decrement()">remove</button>
  <p>Count:{{count}}</p>
  <p></p>
  <div>
</template>


<script>
import HelloWorld from './components/HelloWorld.vue';

export default {
  
  data() {
    return{
    count:0
    }
  },
  methods :{
    increment(){
      this.count++

    },
    decrement(){
      this.count--

    }
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

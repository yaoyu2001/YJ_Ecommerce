<template>
    <div>
      <button v-on:click = "increment">+</button>
      <button v-on:click="decrement">-</button>
      <p><span>{{num}}</span></p>
    </div>
</template>

<script>
  export default {
    props:['num'],
    name: 'HelloWorld',
    data () {
      return {
        // msg: 'Welcome to Your Vue.js App',
        // num:0,
      }
    },
    methods:{
      increment(){
        this.num++
      },
      decrement(){
        this.num--
      }
    }
  }
</script>

<style>

</style>

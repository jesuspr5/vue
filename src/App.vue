<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
       <HelloWorld :msg="count"/>
      
       <button  @click="incremenCont"   >Incrementar +1</button>
       <button @click="decrementCont"> Decrementar -1</button>
        <Buttton :name="nombre" :contador="count" />
  </div> 
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Buttton from './components/Buttton.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    Buttton
}
,
  data: ()=>({
    count : 10,
    nombre:"valor:",
   

  }),
  methods:{
    incremenCont(){
      this.count++
    },
    decrementCont(){
      this.count--
    },
     
  }
  


}
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

button{
 box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2), 0 6px 20px 0 rgba(0,0,0,0.19);;   
background-color: #4CAF50; /* Green */
    color: white;
    border-radius:  4px;
    font-size: 20px;

    margin: 10px;
}
</style>

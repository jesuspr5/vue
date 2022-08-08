<template>
  <div >
    
    <button>{{name}}{{contador}}  </button>
   
  </div>
</template>

<script>




export default {
  name: 'Buttton',
  props: {
    
    name: String,
    contador: Number
    
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>

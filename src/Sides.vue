<template>
  <div>
   <h1>Hey</h1>
   <button @click='send'>Send</button>
  </div>
</template>

<script>
export default {
  data(){
    return{
        message:'coconut'
    }
  },
 
 methods:{
    send(){
        this.$emit('someevent',this.message)
    }
 }
}
</script>

<style>

</style>
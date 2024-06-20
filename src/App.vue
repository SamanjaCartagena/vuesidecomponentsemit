<template>
  <div>
    <sides @someevent='trigger'></sides>
    <p>{{this.message}}</p>
  </div>
</template>

<script>
import Sides from './Sides.vue'
export default {
  emits:['someevent'],
  components:{Sides},
  data(){
    return{
      message:''
    }
  },
  methods:{
    trigger(msg){
      this.message=msg
    }
  }
  

}
</script>

<style>

</style>
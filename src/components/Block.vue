<template>
  <div class="block" v-if="showBlock">
    click me
  </div>
</template>

<script>
export default {
props:['delay'],
data(){
  return {
     showBlock:false
  }
},
mounted(){
  setTimeout(()=>{
     this.showBlock=true
  },this.delay)
},
updated(){

},
unmounted()
{
  
}
}
</script>

<style>

.block {
  width: 400px;
  border-radius:20px;
  background:  #0faf87;
  text-align: center;
  padding: 100px 0 ;
  margin: 40px auto;
}
</style>
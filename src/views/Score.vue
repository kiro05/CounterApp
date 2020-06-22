<template>
  <div class="about">
    <h1>スコアを表示</h1>
    <p>{{ count }}</p>
  </div>
</template>
<script>
 export default {
        date(){
          return{
            // count:'0'
          }
        },
        computed:{
          count(){
            return this.$store.getters.count
          }
        }
 }        
</script>
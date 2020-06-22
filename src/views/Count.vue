<template>
  <div class="about">
    <h1>カウント</h1>
    <p>{{ count }}</p>
    <p>
    <button @click="increment">+</button>
    <button @click="decrement">-</button>
    </p>
  </div>
</template>
    <script>
      export default {
        date(){
          return{
            // count:'0'
          }
        },
        methods:{
          increment(){
            // this.count++,
            this.$store.commit('incriment')
          },
          decrement(){
            // this.count--,
            this.$store.commit('decrement')
          }
        },
        computed:{
          count(){
            return this.$store.getters.count
          }
          
        }
      }
    </script>
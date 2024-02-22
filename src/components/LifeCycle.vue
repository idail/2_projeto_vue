<template>
    <h1>Meu nome é {{ nome }}</h1>
    <!-- <Info /> -->
  </template>
  
  <script>
  import Info from './Info.vue'
  
  export default {
    name: 'LifeCycle',
    components: {
      Info
    },
    data() {
      return { 
        nome: "Ainda não sei"
      }
    },
    created() {
      setTimeout(() => {
        this.nome = "Idail";
      },1000);

      this.lifeCycle();
    },
    mounted(){
      setTimeout(() => {
        this.nome = "Luiz";
      }, 2000);
      this.lifeCycle();
    },
    methods:{
      lifeCycle(){
        console.log("Executou");
      }
    }
  }
  </script>
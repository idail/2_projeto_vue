<template>
    <h1>Meu nome é {{ nome }}</h1>
    <MultiplosEventos/>
    <Reutilizacao/>
    <Reutilizacao/>
    <Reutilizacao/>
    <Reutilizacao/>
  </template>
  
  <script>
  import Info from './Info.vue'
  import MultiplosEventos from "./MultiplosEventos.vue";
  import Reutilizacao from './Reutilizacao.vue';
  export default {
    name: 'LifeCycle',
    components: {
      Info,
      MultiplosEventos,
      Reutilizacao
    },
    data() {
      return { 
        nome: "Ainda não sei"
      }
    },
    created() {
      this.nome = "Matheus"
    }
  }
  </script>
<template>
    <div class="row">
      <div class="col-2">
        <button class="btn btn-primary" @click="decrement">-</button>
      </div>
      <div class="col-8">
        <h2>{{ count }}</h2>
      </div>
      <div class="col-2">
        <button class="btn btn-primary" @click="increment">+</button>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'contadorVue',
    data() {
      return {
        count: 0
      }
    },
    methods: {
      increment() {
        this.count++;
      },
      decrement() {
        if (this.count > 0) {
          this.count--;
        }
      }
    }
  }
  </script>
  
  <style scoped>
  /* Estilos CSS específicos del componente */
  </style>
  
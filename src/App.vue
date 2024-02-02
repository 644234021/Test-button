<script setup>
  import {useCounterStore} from './stores/counter'
  const store = useCounterStore()

  function indrease(){
    store.increment()
  }

  function decrease(){
    store.decrement()
  }
</script>

<template>
  <h1 class="d-flex align-items-center justify-content-center"><b>Count :</b> {{ store.count }}</h1>
  <h1 class="d-flex align-items-center justify-content-center"><b>Double Count :</b> {{ store.doubleCount }}</h1>
  <div class="mt-5 d-grid gap-2 d-flex align-items-center justify-content-center">
    <button type="button" class="btn btn-success btn-lg" @click="indrease()">+ Indrease</button>
    <button type="button" class="btn btn-danger btn-lg" @click="decrease()">- Decrease</button>
  </div>

  
  <div>
  <button type="button" class="btn btn-success btn-lg" @click="indrease()">+ IndreaseX</button>
  <button type="button" class="btn btn-danger btn-lg" @click="decrease()">- DecreaseX</button>
  <button type="button" class="btn btn-info btn-lg">Info</button>
  </div>

  
 
</template>

<style scoped>

</style>


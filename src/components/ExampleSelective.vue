<template>
    <p>{{age }}</p>
    <h1 v-if ="age < 18">Eres menor de edad</h1>
    <h1 v-else>Eres mayor de edad</h1>
    <button @click="addAge">Agregar Edad</button>
</template>

<script lang="ts" setup>
import {Ref, ref, defineComponent} from 'vue';
//Forma con el setup
  let age:Ref = ref(0);
    const addAge = () =>{
        age.value++
    }
//si necesitara la composicion si el setup
/* export default defineComponent({
    name:'ExampleSelective',
    setup: () =>{
        let age:Ref = ref(0);
        const addAge = () =>{
        age.value++
        }
        return {age, addAge}

    }
}) */
  

</script>

<style scoped>
</style>
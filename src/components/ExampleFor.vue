<template>
<ul>
    <li v-for="{code, name} in countries" :key="code">{{ name }}</li>
</ul>
</template>

<script lang="ts" setup>
import {Ref, ref} from 'vue';
interface ICountry{
    code: string,
    name: string
}
let countries:Ref<Array<ICountry>> = ref([
    {
        code: 'es',
        name:'spain'
    },
    {
        code: 'en',
        name:'UK'
    },
    {
        code: 'fr',
        name:'France'
    },
    {
        code: 'it',
        name:'Italy'
    },
    {
        code: 'pt',
        name:'Portugal'
    },
])
</script>

<style scope>
</style>
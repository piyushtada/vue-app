<template>
  <h1> Dc jokers</h1>
  <ul>
    <li v-for="he in dcHeroo" :key="he">  {{he}} </li>
  </ul>
  <form @submit.prevent="dcHeroo.push(newHero)">
    <input v-model="newHero" />
    <button type="submit"> Add hero</button>
  </form>
  </template>

<script>
export default {
  methods:{
    addHero(){
      alert('hooooall');
    }
  },
  data(){
    return{
      attribute: "value",
      isDisabled: 'false',
      dcHeroo: ["so","what","are"],
      newHero: "aquamannn",
    };
  },
  
}
</script>
<script setup lang="ts">
import card from "../components/Card.vue";

const maison = {titre:"Maison v-bind",
 price:34,
  nbrSDB:7,
  nbrLit:8,
   taille:100,
    image:"/images-maison/maison2.jpg"}
</script>

<template class="bg-indigo-25">
  <div class="flex">
    <card
      class="w-1/2"
      :favoris="true"
      image="/images-maison/maison1.jpg"
      titre="Maison simple"
      nbrSDB="2"
      taille=200
      nbrLit=7
    />
    <card class="w-1/2" v-bind="maison"/>
  </div>
</template>



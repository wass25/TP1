<script setup lang="ts">
import card from "../components/Card.vue";

const res = await fetch("/maisons.json");
const listeMaisons = await res.json();
console.log(listeMaisons);

</script>
<template>
    <div class="p-2">
        <div v-for="uneMaison in listeMaisons" :key="uneMaison.titre">
            <card class="w-1/2" v-bind="uneMaison" />
        </div>
    </div>
</template>

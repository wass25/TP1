<script setup lang="ts">
import card from "../components/Card.vue";

const res = await fetch("/maisons.json");
const listeMaisons = await res.json();

</script>
<template>
    <div class="flex">
        <div v-for="uneMaison in listeMaisons" :key="uneMaison.titre">
            <card class="w-1/2" v-bind="uneMaison" />
        </div>
    </div>
</template>

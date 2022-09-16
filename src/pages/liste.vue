<script setup lang="ts">
import card from "../components/Card.vue";
import maisons from "../assets/maisons.json";
</script>
<template>
    <div class="flex">
        <div v-for="maison in maisons" :key="maison.titre">
            <card class="w-2/2" v-bind="maison" />
        </div>
    </div>
</template>
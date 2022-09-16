<script>
import card from "../components/Card.vue";
export default {
  name: "App",
  components: { card },
};
</script>

<template class="bg-indigo-25">
  <div class="grid grid-flow-row-dense grid-cols-[repeat(auto-fit,minmax(340px,1fr))]">
    <card
      class="p-8"
      :favoris="true"
      image="/images-maison/maison1.jpg"
      titre="Beverly Springfield"
      lieu="2821 Lake Sevilla, Palm Harbor, TX"
      nbrSDB="2"
    />
  </div>
</template>


<template>
  <section class="grid-container">
    <ApartmentCard
      v-for="apt in apartments"
      :key="apt.id"
      :apartment="apt"
    />
  </section>
</template>

<script setup>
import apartments from '../data/apartments';
import ApartmentCard from '../components/ApartmentCard.vue';
</script>

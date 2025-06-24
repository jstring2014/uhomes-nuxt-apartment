<template>
  <div class="card">
    <img :src="apartment.image" alt="apartment" />
    <h2>{{ apartment.title }}</h2>
    <p>{{ apartment.city }} • {{ apartment.type }}</p>
    <p class="price">¥{{ apartment.price.toLocaleString() }}/month</p>
  </div>
</template>

<script setup>
defineProps({
  apartment: Object
});
</script>

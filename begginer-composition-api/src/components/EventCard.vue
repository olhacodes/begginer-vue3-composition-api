<script setup>
import { ref } from 'vue';
// defineProps({
//   msg: {
//     type: String,
//     required: true
//   }
// })
const event = ref({
  id: 14353,
  title: 'Vue.js Workshop',
  date: '2021-09-01',
  time: '10:00',
  location: 'Online',
  description: 'Join us for a full day of Vue.js training and fun!',
  category: 'workshop',
  organizer: 'Vue School',
  freeEnterance: true
})
</script>

<template>
  <div class="event-card">
    <h2>{{ event.title }}</h2>
    <span>@ {{ event.time }} on {{ event.date }}</span>
  </div>
</template>

<style scoped>
.event-card {
  padding: 20px;
  width: 250px;
  cursor: pointer;
  border: 1px solid #39495c;
  margin-bottom: 18px;
}
.event-card:hover {
  transform: scale(1.01);
  box-shadow: 0 3px 12px 0 rgba(0, 0, 0, 0.2);
}
</style>

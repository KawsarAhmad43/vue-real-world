<template>
  <div class="events">
    <img alt="Vue logo" src="../assets/logo.png" />
    <EventCard v-for="event in events" :key="event.id" :event="event" />
  </div>
</template>

<script>

import EventCard from "@/components/EventCard.vue";

export default {
  name: "HomeView",
  components: {
    EventCard,
  },
  data(){
    return{
      events: [
        {
          id: 123,
          category: 'dummy category',
          title: 'dummy title',
          description: 'dummy description',
          location: 'dummy location',
          date: 'March 5, 2023',
          time: '5:00',
          petsAllowed: true,
          organizer: 'dummy mia'
        },
        {
          id: 345,
          category: 'dummy category',
          title: 'Sarfaraz er Biye',
          description: 'dummy description',
          location: 'dummy location',
          date: 'March 5, 2023',
          time: '5:00',
          petsAllowed: true,
          organizer: 'dummy mia'
        },
        {
          id: 678,
          category: 'dummy category',
          title: 'Sadia apur Biye',
          description: 'dummy description',
          location: 'dummy location',
          date: 'March 5, 2023',
          time: '5:00',
          petsAllowed: true,
          organizer: 'dummy mia'
        },
      ]
    }
  }
};
</script>


<style scoped>
  .events{
    display:flex;
    flex-direction: column;
    align-items: center;
    
  }
  
</style>

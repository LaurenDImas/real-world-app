<template>
  <h1>Evenets For Good</h1>
  <div class="events">
    <EventCard v-for="event in events" :key="event.id" :event="event" />
  </div>
</template>

<script>
// @ is an alias to /src
import EventCard from "@/components/EventCard.vue";
export default {
  name: "EventList",
  components: {
    EventCard,
  },
  data() {
    return {
      events: [
        {
          id: 5928101,
          category: "animalwlfare",
          title: "Cat Adoption Day",
          description: "Find your new feline friend at this event 1",
          location: "Meow Town",
          date: "January 28, 2022",
          time: "12:00",
          petsAllowed: true,
          organizer: "Kat Laydee",
        },
        {
          id: 5928102,
          category: "food",
          title: "Food Adoption Day",
          description: "Find your new feline friend at this event 2",
          location: "Meow Town",
          date: "January 28, 2022",
          time: "12:00",
          petsAllowed: true,
          organizer: "Kat Laydee",
        },
        {
          id: 5928103,
          category: "sustainability",
          title: "Sustainability Adoption Day",
          description: "Find your new feline friend at this event 3",
          location: "Meow Town",
          date: "January 28, 2022",
          time: "12:00",
          petsAllowed: true,
          organizer: "Kat Laydee",
        },
      ],
    };
  },
};
</script>
<style scoped>
.events {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>

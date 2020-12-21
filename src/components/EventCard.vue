<template>
  <div class="event-card">
    <!-- Display event data -->
    <span>@ {{ event.time }} on {{ event.date }}</span>
    <h4>{{ event.title }}</span>
  </div>
</template>

<script>
export default {
  name: "EventCard",
  // props: {
  //   msg: String
  // }
  data() {
    return {
      event: {
        id: 123456,
        category: 'animal welfare',
        title: 'Cat Adoption Day',
        description: 'Find your new feline friend at this event.',
        location: 'Meow Town',
        date: 'December 21, 2020',
        time: '12:00',
        petsAllowed: true,
        organizer: 'Erik Mortimer'
      }
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
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
  box-shadow: 0 3px 13px 0 rgba(0, 0, 0, 0.2);
}
</style>

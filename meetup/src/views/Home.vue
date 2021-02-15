<template>
  <div class="home">
    <h2>Meetings</h2>
    <MeetingItems v-for="meeting in displayMeeting" :key="meeting.id" :meeting="meeting" />
  </div>
</template>

<script>
import MeetingItems from "../components/MeetingItems"
export default {
  name: "Home",
  components: { 
    MeetingItems
   },
  computed: {
    displayMeeting() {
      return this.$store.state.meeting
    }
  }
};
</script>

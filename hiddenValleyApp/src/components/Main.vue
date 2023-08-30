<script>import WorkshopTimetable from './WorkshopTimetable.vue'
 export default {
  components: {
    WorkshopTimetable // Register the Workshop Timetable component
  },
  data() {
    return {
    };
  },
  methods: {
  }
};
</script>

<template>
  <div class="main">
    <div class="main-container">
      <div class="main-heading">
        <h1>Hidden Valley</h1>
        <h2>Sustainable Living Workshops</h2>
        </div>
        <div class="main-other">
        <div class="main-left">
          <WorkshopTimetable />
        </div>
        <div class="main-right">
          <ul class="main-text">
            <li class="main-li">Are you looking for inspiration and information to start gardening, bread baking, making compost or building? You might want to extend your knowledge and improve your practical skills. Or you might be travelling in Tasmania and looking for an interesting activity to do while you are here. </li>
            <li class="main-li">Our workshops will inspire you to get out there and start that new hobby or project you want to do, and they are a fun and informative way to spend your Sunday morning! </li>
            <li class="main-li">Hidden Valley is only 20 minutes from Deloraine, an hour from Devonport or Launceston, and 2 hours from Hobart on the Great Lakes touring route.</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>


<template>
  <div class="content">
    <h3>Coming up:</h3>
    <table>
      <thead>
        <tr>
          <th>Date</th>
          <th>Workshop</th>
        </tr>
      </thead>
      <tbody>
        <!-- Loop through each workshop in 'workshops' array -->
        <tr v-for="(workshop, index) in workshops" :key="index">
          <td>{{ workshop.date }}</td> <!-- Display workshop date -->
          <td><a class="workshop-a" :href="workshop.link" @click="trackClick(index)">{{ workshop.name }}</a></td> <!-- Display workshop name as a link -->
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  data() {
    return {
      // Array of workshop objects with details
      workshops: [
        { date: "11 February 2024", name: "No Dig Gardening", link: "#", clickedDate: null },
        { date: "18 February 2024", name: "Basic Building Skills for Women", link: "#", clickedDate: null },
        { date: "3 March 2024", name: "Sourdough Bread for Beginners", link: "#", clickedDate: null },
        { date: "17 March 2024", name: "Polytunnel and Greenhouse Growing", link: "#", clickedDate: null },
        { date: "24 March 2024", name: "Keeping Chooks for Eggs", link: "#", clickedDate: null },
        { date: "7 April 2024", name: "Compost Making and Worm Farms", link: "#", clickedDate: null },
      ],
      clickCounts: Array.from({ length: 6 }, () => 0) // // Array to store click counts
    };
  },
  methods: {
    trackClick(index) {
      this.clickCounts[index]++; // Increment click count for the clicked link
      this.workshops[index].clickedDate = new Date().toLocaleDateString(); // Capture the clicked date
    }
  }
};
</script>

<style scoped>
/* Scoped styles for the component */
th, td {
  border: 1px solid white;
  padding: 12px;
  text-align: center;
  background-color: white;
  color: black;
  
}

th {
  font-weight: bold;
  background-color: #0E6251;
  color: white;
}

.workshop-a {
  color: black;
  text-decoration: none;
  padding: 10px;
  transition: background-color 0.3s;
}

.workshop-a:hover {
  background-color: #f0f0f0;
}

table {
  width: 100%;
}
</style>
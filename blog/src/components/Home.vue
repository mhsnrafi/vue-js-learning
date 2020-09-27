<template>
  <div>
    <!-- <h1 v-if="show">Conditional Rendereing in Vue js</h1>
     <h1 v-else>Conditional Rendereing Else</h1>
    <button v-on:click="display">Toggle Element</button>-->
    <!-- <h2>{{ data }}</h2>
    <h2>{{ msg }}</h2>-->
    <!-- <button v-on:click="hello"> Call Hello Function</button> -->
    <h1>For Loop in Vue.js</h1>
    <table>
      <tr>
        <td>ID</td>
        <td>Name</td>
        <td>Email Address</td>
      </tr>
      <tr v-for="user in users" :key="user.id">
        <td>{{ user.id}}</td>
        <td>{{ user.name}}</td>
        <td>{{ user.email}}</td>
      </tr>
    </table>
  </div>
</template>

<script>
export default {
  name: "Home",
  props: {
    data: String,
    msg: String
  },
  methods: {
    hello() {
      console.log("HELLO Testing method");
    },
    display() {
      this.show = !this.show;
    }
  },
  data() {
    return {
      show: true,
      users: [
        { id: 1, name: "Mohsin", email: "mohsin@gmail.com" },
        { id: 2, name: "John", email: "John@gmail.com" },
        { id: 3, name: "Peter", email: "Peter@gmail.com" },
        { id: 4, name: "Tony", email: "moTonyhsin@gmail.com" }
      ]
    };
  }
};
</script>


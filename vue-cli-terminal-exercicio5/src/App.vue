<template>
  <div id="app">
    <span> fullNameComputed: {{ fullNameComputed }}</span> 
    <br>
    <span> fullNameMethods: {{ fullNameMethods()}}</span>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      firstName: "Harry",
      lastName: "Potter",
    };
  },
  computed: {
    fullNameComputed() {
      return `${this.firstName}  ${this.lastName}`;
    },
  },
  methods: {
    fullNameMethods() {
      return `${this.firstName}  ${this.lastName}`;
    },
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

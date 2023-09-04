<template>
  <div id="app">
    <h1>Hello</h1>
  </div>
</template>

<script>
import Vue from "vue";
import Component from "vue-class-component";
// import StarRating from "./components/StarRating";

// Define the component in class-style
@Component({
  name: "app",
  props: [
    "name",
    "displayLabel",
    "disabled",
    "value",
    "fieldDesc",
    "placeholder",
    "focus",
    "customClass",
    "required",
    "fluid",
    "noValidationOnBlur",
    "isMultiDecimalField",
  ],
  components: {},
})
export default class App extends Vue {
  // Class properties will be component data
  count = 0;

  // Methods will be component methods
  increment() {
    this.count++;
  }

  decrement() {
    this.count--;
  }
}
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

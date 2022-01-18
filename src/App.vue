<template lang="pug">
  <div id="app">
    FormHelper
      div(slot="form-header")
        h3 This is form title
        p Information is here
      div(slot="form-fields")
        input(type="text" placeholder="name" required)
        input(type="password" placeholder="password" required)
      div(slot="form-controller")
        button(@click="handleSubmit") Submit

  </div>
</template>

<script>
import FormHelper from "./components/FormHelper.vue"

export default {
  name: "App",
  components: {
    FormHelper,
  },
  methods: {
    handleSubmit: function () {
      alert("Complete!")
    },
  },
}
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

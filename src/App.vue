// App.vue

<template lang="pug">
  <div id="background">
    <div id="box">
      <p>{{name}}</p>
      <span>I want to buy </span>
      <button v-on:click="fruit--">-</button>
      <span>{{fruit}}</span>
      <button v-on:click="fruit++">+</button>
      <span> bananas.</span>
      <p>Shannon and {{name}} want to buy {{fruit}} bananas.</p>
      <button v-on:click="dollar--">$</button>
      <span>{{dollar}}</span>
      <button v-on:click="dollar++">$$</button>
      <br/><button v-on:click="name = 'Baby Yoda'">change name</button>
    </div>
  </div>
</template>

<script>
import Vue from "vue";
export default Vue.extend({
  data() {
    return {
      fruit: 2,
      name: "Amanda Lorian",
      dollar: 500
    };
  },
  methods: {}
});
</script>
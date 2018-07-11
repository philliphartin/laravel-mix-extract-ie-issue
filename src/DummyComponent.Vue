<template>
    <button v-on:click="onClick">
        <span>Click me {{ count }} </span>
    </button>
</template>

<script>
export default {
  name: "dummy-component",
  data() {
    return {
      count: 0
    };
  },
  methods: {
    onClick() {
      console.log("I've been clicked");
      this.count = this.count + 1;
    }
  },
  mounted: function() {
    console.log("DummyComponent mounted");
  }
};
</script>

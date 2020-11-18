<template>
  <div id="front">
    <div class="home">
      <h1>{{ message }}</h1>
    </div>
  </div>
</template>

<style>
#front {
      margin: 0;
      padding: 0;
      width: 100vw;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    canvas {
      position: absolute;
    }
</style>

<script>
export default {
  data: function() {
    return {
      message: "Welcome to Serenity"
    };
  },
  created: function() {},
  methods: {}
};
</script>
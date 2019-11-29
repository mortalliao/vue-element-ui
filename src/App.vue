<template>
  <div id="app">
    <div>
      <p>
        {{count}}
      </p>
      <el-button @click="plus" type="primary" size="small">el-button</el-button>
      <el-button @click="minus">el-button</el-button>
    </div>
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "app",
  data(){
    return {
       count: 0
    }
  },
  components: {
  },
  methods:{
    plus(){
      this.count++
    },
    minus(){
      this.count--;
    }
  }
};
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

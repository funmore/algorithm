<template>
<!-- <div>
    <img alt="Vue logo" src="./assets/logo.png"> -->
    <div>
    <span> father msg:    {{fatherMsg}}</span>

    <props-change :PropMsg="fatherMsg"></props-change>
    <button @click="onFatherClick">father button</button>
  </div>
</template>

<script>
// import Algorithm from './components/Algorithm.vue'
// import VueFrame from './components/VueFrame.vue'
// import PromiseTest from './components/PromiseTest.vue'
// import PropsChange from './components/PropsChange.vue'
export default {
  name: 'app',
  components: {
    // Algorithm,
    // VueFrame
    // PromiseTest,
    // PropsChange
    
  },
  data(){
    return {
      fatherMsg:0
    };
  },
  methods:{
    onFatherClick(){
      this.fatherMsg=Math.random();
    }
  }
    
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    
    <Layout></Layout>
    <queue></queue>

     <h3 id="h3Brew">Light</h3>
  <input type="checkbox" data-toggle="toggle" data-on="Off" data-off="On" id="toggle">
  </div>
</template>


  

<script>
import queue from './submodules/queue/src/App.vue'
import Layout from'./submodules/base_layout/src/components/interface'


export default {
  name: 'App',
  components: {
    queue,
    Layout
  }
}


  // var socket = io.connect();
  // (function() {
  // ('#toggle').bootstrapToggle({
  //     on: 'ON',
  //     off: 'OFF'
  //   });
  // })
        // ("#toggle").change(function(){
        //   if(("#toggle").prop("checked") == true){
        //    socket.emit('lightOn', 'on\n');
        //   }else{
        //    socket.emit('lightOff', 'off\n');}
        //  });

        // socket.on('lightOn', function() {
        //   ('#toggle').bootstrapToggle('on');
        // });
        //  socket.on('lightOff', function() {
        //   ('#toggle').bootstrapToggle('off');
        // });

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

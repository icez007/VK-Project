<template>
  <div id="app">
    <Kanban :data="data"/>    
  </div>
</template>

<script>
import Kanban from "./components/Kanban"

export default {
  name: 'App',
  components: {
    Kanban
  },
  data(){
    return{
      data:[
        {
          name:"todo",
          color: "#BB8FCE",
          tasks:[]
        },
        {
          name:"doing",
          color: "#85C1E9",
          tasks:[]
        },
        {
          name:"done",
          color: "#82E0AA",
          tasks:[]
        }
      ]
    }
  }
}
</script>

<style>
#app {
  height: 100vh;
}
</style>

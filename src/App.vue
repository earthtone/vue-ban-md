<template>
  <div id="app">
    <todo-list/>
    <doing-list/>
    <done-list/>
  </div>
</template>

<script>
import TodoList from './tasks/TodoList.md'
import DoingList from './tasks/DoingList.md'
import DoneList from './tasks/DoneList.md'

export default {
  name: 'app',
  components: {
    TodoList,
    DoingList,
    DoneList
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;

  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
}

section {
  border: 1px solid #aaa;
  height: 100%;
  padding: 1rem;
  margin: 0.5rem;
}
</style>

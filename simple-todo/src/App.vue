<template>
  <div id="app">
    <CompletedTodos></CompletedTodos>
    <CurrentTodos></CurrentTodos>
    <CreateTodo></CreateTodo>
  </div>
</template>

<script>
import CreateTodo from './components/CreateTodo'
import CurrentTodos from './components/CurrentTodos'
import CompletedTodos from './components/CompletedTodos'
export default {
  name: 'App',
  components: {
    CreateTodo,
    CurrentTodos,
    CompletedTodos
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>

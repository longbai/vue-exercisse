<template>
  <div id="get-todo" class="container">
    <input class="form-control" :value="newTodo" placeholder="I need to...." @change="createTodo">
    <button class="btn btn-primary" @click="addTodo">Add Todo</button>
  </div>
</template>

<script>
export default {
  methods: {
    createTodo (e) {
      this.$store.dispatch('createTodo', e.target.value)
    },
    addTodo () {
      this.$store.dispatch('addTodo')
      this.$store.dispatch('clearTodo')
    }
  },
  computed: {
    newTodo () {
      return this.$store.getters.newTodo
    }
  }
}
</script>

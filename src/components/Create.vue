<template>
  <div>
    <input type="text" v-model="createTodo" />
    <button @click='onSaveButtonClick'>save</button>
  </div>
</template>

<script>
export default {
  name: 'Create',
  data: () => ({
    createTodo: '',
  }),
  props: ['todos'],
  methods: {
    onSaveButtonClick() {
      this.todos.push({
        text: this.createTodo,
      });
      this.createTodo = '';
    },
  },
};
</script>

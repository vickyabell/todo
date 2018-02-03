<template>
  <div id="app">
    <Header />
    <Create :todos='todos' />
    <Todos :todos='todos'  />
  </div>
</template>

<script>
import Header from '@/components/Header';
import Create from '@/components/Create';
import Todos from '@/components/Todos';

export default {
  name: 'App',
  components: {
    Header,
    Create,
    Todos,
  },
  data: () => ({
    todos: [],
  }),
};
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

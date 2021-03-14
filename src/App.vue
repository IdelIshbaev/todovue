<template>
  <div id="app todo">
    <h1>To do App</h1>
    <input v-model="todo" type="text" placeholder="Type to do..."/>
    <button @click="addToDo(id++)">Add to the list</button>
    <!-- <todoamount :todos="todos"/> -->
    <todolist :todos="todos"  @removeTodo="removeTodo" />
  </div>
</template>

<script>
import todolist from './components/todolist.vue';
export default {
  name: 'App',
  components:{
    todolist
    // todoamount
  },
  data(){
     return{
      todo: "",
      todos: [],
      isDone: false,
      id: 0
    }
  },
  mounted(){
    const data = localStorage.getItem("todos")
    if(data){
      this.todos = JSON.parse(data)
    }
  },
  methods: {
    addToDo(){
      if(this.todo != ''){
        this.todos.push({
          id: this.id,
          text: this.todo,
          isComplete: this.isDone
        });
        localStorage.setItem("todos", JSON.stringify(this.todos));
      }
      this.todo = "";
    },
    removeTodo(index){
      this.todos.splice(index, 1);
      localStorage.setItem("todos", JSON.stringify(this.todos));
    }
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.title{
  text-align: center;
  margin-top: 60px;
}
.todo{
  height: 100%;
  padding: 30px;
}
.todo_id{
  font-weight: bold;
}
.todo_text{
  text-transform: capitalize;
}
.isShow{
  color: grey;
  text-decoration: line-through;
}
</style>

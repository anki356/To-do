<template>
  <div >
      <input type="text" class="todo-input" placeholder="What needs to be done" v-model="newTodo" @keyup.enter="addTodo">
      <div v-for="todo in todos" :key="todo.id" class="todo-item">
          {{todo.title}}
          </div>
      
  </div>
</template>

<script>
export default {
  name: 'todo',
  data () {
    return {
        todos:[
            { newTodo: '',
             'id':1,
              'title':'',
              'completed':false,
          },
        ]
    }
  },
          methods : {
          addTodo(){
            this.todos.push({
                id: this.id,
                title: this.newTodo,
                completed:false,
            })
          
      

this.newTodo=" "
this.id++
          }
          }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style >

</style>

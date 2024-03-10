<template lang="">
 <div class="flex flex-col items-center justify-center mt-20 text-[1.6rem]">
    <input type = "text" v-model = "newTask" class="border-[1px] border-black border-solid">
    <button @click="addTask">Add</button>
      <div v-for = "(task, index) in tasks" :key="index" >
           <input type ="checkbox" v-model= "task.status"  > 
           <span :class="{done: task.status}">{{task.content}}</span>
           <button @click="deleteTask(index)" class="mx-4">Delete</button>
            <button  @click="updateTask(index)">Update</button>
            <button @click="saveTask(index)">Save</button>
        </input>
      </div>
 </div>
</template>
<script>
export default {
  name: "todo-list",
  data() {
    return {
    
    tasks: [
      { content: "Chill with code", status: false },
      { content: "Learning VueJS", status: false },
      { content: "Learning English", status: false },
      { content: "Reading Book", status: false },
    ],
    newTask: ""
    }
  },

  methods: {
    addTask() {
      if (this.newTask.trim() !== '') {
        this.tasks.push({ content: this.newTask, status: false });
        this.newTask = '';
      }
    },
    deleteTask(index) {
      if(this.tasks[index].status === true) {
        this.tasks.splice(index,1)
      }
      },
     updateTask(index) {
         this.newTask = this.tasks[index].content 
      
    },
    saveTask(index) {
      if (this.newTask !== "") {
         this.tasks[index].content = this.newTask
         this.newTask = ""
      }
    }
  }

};
</script>
<style lang="scss">
    .done {
    text-decoration-line: line-through
    }
</style>






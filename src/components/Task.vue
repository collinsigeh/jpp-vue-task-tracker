<script>
    export default {
        name: 'Task',
        props: {
            task: Object
        }
    }
</script>

<template>
    <div :class="[task.reminder ? 'reminder' : '', 'task']">
        <h1>{{ task.text }} <i class="fas fa-times-circle"></i></h1>
        <p>{{ task.day }}</p>
    </div>
</template>

<style scoped>
.fas {
  color: red;
}
.task {
  background: #f4f4f4;
  margin: 5px;
  padding: 10px 20px;
  cursor: pointer;
}
.task.reminder {
  border-left: 5px solid green;
}
.task h3 {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
</style>
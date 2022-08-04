<script>
import Task from './Task.vue';

export default {
    name: "Tasks",
    props: {
        tasks: Array
    },
    emits: [
        'delete-task-go',
        'toggle-task-go'
    ],
    components: { Task }
}
</script>

<template>
    <div v-for="task in tasks" :key="task.id">
        <Task @toggle-task="$emit('toggle-task-go', task.id)" @delete-task="$emit('delete-task-go', task.id)" :task="task" />
    </div>
</template>


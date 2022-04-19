<template>
    <header>
       <h1>{{title}}</h1> 
       <Button @btn-click="$emit('toggle-task-form')" :title="showAddTask ? 'Close' : 'Add Task'" :color = "showAddTask ? 'red' : 'green'" />
    </header>
</template>

<script>

import Button from './Button'

export default{
    name: 'Header',
    props: {
        title: String,
        showAddTask: Boolean
    },
    components: {
        Button
    },
    emits: ['toggle-task-form']
}
</script>

<style scoped>
header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
}
</style>

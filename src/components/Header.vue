<script>
    export default {
        name: 'Header',
        props: {
            title: {
                type: String,
                default: 'Collins Igeh App'
            }
        }
    }
</script>

<template>
    <header>
        <h1>{{ title }}</h1>
    </header>
</template>

<style scoped>
    header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 20px;
    }
</style>
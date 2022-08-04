<script>
    import Button from "./Button.vue";

    export default {
        name: 'Header',
        props: {
            title: {
                type: String,
                default: 'Collins Igeh App'
            }
        },
        components: {
            Button
        }
    };
</script>

<template>
    <header>
        <h1>{{ title }}</h1>
        <Button />
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
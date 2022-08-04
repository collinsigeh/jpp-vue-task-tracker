<script>
    export default {
        name: 'Button',
        props: {
            text: {
                type: String,
                default: 'Button'
            },
            color: {
                type: String
            }
        }
    }
</script>

<template>
    <button class="btn" :style="{ backgroundColor: color }">{{ text }}</button>
</template>
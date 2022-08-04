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
        },
        methods: {
            onClick() {
                console.log('Clicked')
            }
        }
    }
</script>

<template>
    <button class="btn" :style="{ backgroundColor: color }" @click="onClick">{{ text }}</button>
</template>
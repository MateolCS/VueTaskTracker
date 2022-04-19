<template>
    <button @click="$emit('btn-click')" :style="{background: color}" class="btn">{{title}}</button>
</template>

<script>
export default{
    name: 'Button',
    props: {
        title: String,
        color: {
            type: String,
            default: '#000'
        },
    }
}
</script>

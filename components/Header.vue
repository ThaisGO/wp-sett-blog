<script setup>
    const props = defineProps({
        title: String,
        subtitle: String
    })
</script>

<template>
    
    <div>
        <div>
            <h1>{{  title }}</h1>
            <h3>{{ subtitle }}</h3>
        </div>
    </div>
</template>
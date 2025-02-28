<script setup>
    const route = useRoute()
</script>

<template>
    <h1>dinamic route: {{ route.params.slug }}</h1>
</template>
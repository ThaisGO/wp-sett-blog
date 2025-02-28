<script setup>
import { ref } from 'vue';

    const { params } = useRoute()
    const slug = ref('')

    // if(route.params.slug) {
    //     let lastIndex = route.params.slug.length - 1
    //     if(!route.params.slug[lastIndex]) {
    //         slug.value = route.params.slug[lastIndex -1]
    //     } else {
    //         slug.value = route.params.slug[lastIndex]
    //     }
    // } else {
    //     slug.value = 'home'
    // }

    // const { data, pending, error, refresh } = await useFetch('https://sett.thaisgodev.com/wp-json/wp/v2/pages', {
    //     query: { slug: slug.value }
    // })

    // const {data: posts } = await useFetch('https://sett.thaisgodev.com/wp-json/wp/v2/posts')
</script>

<template>
    <!-- <Header :title="data[0].title.rendered" :subtitle="data[0].content.rendered" />

    <div v-for="post in posts" :key='post.id'>
        <h1 class="bg-red-500">{{ post.title.rendered }}</h1>
        <p>{{ post.excerpt.rendered }}</p>
        <p>{{ post._links['wp:attachment'][0].href }}</p>
        <img v-if="post.acf && post.acf.upload_imagem" :src="post.acf.upload_imagem" :alt="post.title.rendered" class="max-h-80">

    </div> -->
</template>
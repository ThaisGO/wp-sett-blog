<script setup>
import { ref } from 'vue';
// import Header from '~/components/Header.vue';

    const route = useRoute()
    const slug = ref('')

    if(route.params.slug) {
        let lastIndex = route.params.slug.length - 1
        if(!route.params.slug[lastIndex]) {
            slug.value = route.params.slug[lastIndex -1]
        } else {
            slug.value = route.params.slug[lastIndex]
        }
    } else {
        slug.value = 'home'
    }

    const { data, pending, error, refresh } = await useFetch('https://sett.thaisgodev.com/wp-json/wp/v2/pages', {
        query: { slug: slug.value }
    })
</script>

<template>
    <!-- <div v-if="data && data.length"> -->
        <Header :title="data[0].title.rendered" :subtitle="data[0].content.rendered" />
    <!-- </div> -->


    <!-- <h1>{{data[0].title.rendered}}</h1> -->
    <!-- <div>

        <div> {{ data[0].content.rendered }}</div>
        <div> {{ data }}</div>
    </div> -->
</template>
<template>
    <nav class="bg-zinc-900 text-white p-3 ">
        <div class="container flex justify-around items-center">
        <div class="">
            <h1>World News</h1>
            <!-- <img src="" alt="" class="w-full"> -->
        </div>
        <ul class="inline-flex gap-2">
            <li><NuxtLink to="/">Home</NuxtLink></li>
            <li><NuxtLink to="/categories">Categories</NuxtLink></li>
        </ul>
        <div>
            <ul class="inline-flex gap-2">
                <li>In</li>
                <li>Tw</li>
                <li>Yt</li>
            </ul>
        </div>
        </div>
    </nav>
</template>

<script>
export default {
    setup () {
        

        return {}
    }
}
</script>

<style lang="scss" scoped>

</style>
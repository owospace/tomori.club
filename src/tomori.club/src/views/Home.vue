<template>
    <div id="home">
        <HomeBanner />
        <Staff />
        <HomeSeparator />
        <News />
        <About />
    </div>
</template>

<script>
import HomeBanner from '@/components/HomeBanner.vue'
import Staff from '@/components/Staff.vue'
import HomeSeparator from '@/components/HomeSeparator.vue'
import News from '@/components/News.vue'
import About from '@/components/About.vue'

export default {

    name: "Home",
    
    data() {
        return {
            loading: true,
            title: 'Home'
        };
    },

    components: {
        HomeBanner,
        Staff,
        HomeSeparator,
        News,
        About,
    },

    created() {
        const title = this.title + ' @ tomori.club'
        if (title) {
            document.title = title
        }
    },

    mounted() {
        setTimeout(() => {
            this.loading = false;
        }, 1200);
    },

};
</script>

<style>

</style>
<template>
    <div class="newswrapper__news">
        <div class="cheading">
            <span class="cheading--main">
                Latest News
            </span>
            <span class="cheading--sub">
                <a href="#">see all</a>
            </span>
        </div>
        <div>
            <div class="row">
                <div class="col-md-4" v-for="(n, i) in news.slice(0, 3)" :key="i"> 
                    <app-ncard  :src="n.src" :link="n.link" :heading="n.heading" :time="n.time"/>
                </div>
            </div>
        </div> 
    </div>
</template>

<script>

import ncard from '~/components/news_card'

export default {
    components: {
        'app-ncard': ncard 
    },
    data() {
        return {
            news: [
                {
                    src: '/07.jpg',
                    link: '#',
                    heading: 'laborumSunt non sunt exercitation ex',
                    time: Date.now()
                },
                {
                    src: '/14.jpg',
                    link: '#',
                    heading: 'consectetur et cupidatat cillum cupidatat dui',
                    time: Date.now()
                },
                {
                    src: '/2.jpg',
                    link: '#',
                    heading: 'Veniam laborum tempor labore non laborumSun exe',
                    time: Date.now()
                },
                {
                    src: '/09.jpg',
                    link: '#',
                    heading: 'there is no heading',
                    time: Date.now()
                }
            ]

        }
    },
    mounted() { 
    }
}
</script>

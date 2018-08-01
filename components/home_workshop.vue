<template>
    <div class="newswrapper__workshop">
        <div class="cheading">
            <span class="cheading--main">
                Workshops and Seminars
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
                    src: '/09.jpg',
                    link: '#',
                    heading: 'Engineering Workshop – 2018 Organized by ChE',
                    time: Date.now()
                },
                {
                    src: '/06.jpg',
                    link: '#',
                    heading: 'Seminar on – Jute and Jute Industries”',
                    time: Date.now()
                },
                {
                    src: '/12.jpg',
                    link: '#',
                    heading: 'Workshop on – Recent Trends in Biotechnology',
                    time: Date.now()
                },
                {
                    src: '/12.jpg',
                    link: '#',
                    heading: 'there is no heading',
                    time: Date.now()
                }
            ]

        }
    }
}
</script>

<template>
    <div class="section__workshop">
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
                    src: 'http://loremflickr.com/400/400',
                    link: '#',
                    heading: 'there is no heading',
                    time: Date.now()
                },
                {
                    src: 'http://loremflickr.com/400/400',
                    link: '#',
                    heading: 'there is no heading',
                    time: Date.now()
                },
                {
                    src: 'http://loremflickr.com/400/400',
                    link: '#',
                    heading: 'there is no heading',
                    time: Date.now()
                },
                {
                    src: 'http://loremflickr.com/400/400',
                    link: '#',
                    heading: 'there is no heading',
                    time: Date.now()
                }
            ]

        }
    }
}
</script>

<template>
    <div class="notice">
        <div class="notice__header">
            <div class="cheading">
                <span class="cheading--main">
                    Notice Board
                </span>
                <span class="cheading--sub">
                    <a href="#">see all</a>
                </span>
            </div>
        </div>
        <div class="notice__content">
            <ul>
                <li class="notice__content--item" v-for="(n, i) in notices" :key="i">
                    <div class="notice__card d-flex justify-content-between">
                        <div class="notice__card--time">
                            <span class="notice__card--time--date">{{ n.time | moment("DD") }}</span>
                            <span class="notice__card--time--month">{{ n.time | moment("MMM") }}</span>
                        </div>
                        <div class="notice__card--content">
                            <span class="notice__card--content-title"> {{ n.title }} </span> 
                            <nuxt-link class="notice__card--content-link" :to="n.link"> show </nuxt-link>
                        </div>
                    </div>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            notices: [
                {
                    time: Date.now(),
                    title: 'List of Selected Candidates for the post of Assistant Professor and Lecturer of Petroleum and Mining Engineering ',
                    link: '#'
                },
                {
                    time: Date.now(),
                    title: 'বায়ো মেডিকেল ইঞ্জিয়ারিং বিভাগের সহকারী অধ্যাপক ও প্রভাষক নিয়োগ নির্বাচনী পরীক্ষা অনিবার্য কারনবশত স্থগিত',
                    link: '#'
                },
                {
                    time: Date.now(),
                    title: 'List of Selected Candidates for the post of Assistant Professor and Lecturer of Petroleum and Mining Engineering ',
                    link: '#'
                },
                {
                    time: Date.now(),
                    title: 'বায়ো মেডিকেল ইঞ্জিয়ারিং বিভাগের সহকারী অধ্যাপক ও প্রভাষক নিয়োগ নির্বাচনী পরীক্ষা অনিবার্য কারনবশত স্থগিত',
                    link: '#'
                },
                {
                    time: Date.now(),
                    title: 'List of Selected Candidates for the post of Assistant Professor and Lecturer of Petroleum and Mining Engineering ',
                    link: '#'
                },
                {
                    time: Date.now(),
                    title: 'List of Selected Candidates for the post of Assistant Professor and Lecturer of Petroleum and Mining Engineering ',
                    link: '#'
                },
                {
                    time: Date.now(),
                    title: 'List of Selected Candidates for the post of Assistant Professor and Lecturer of Petroleum and Mining Engineering ',
                    link: '#'
                },
                {
                    time: Date.now(),
                    title: 'List of Selected Candidates for the post of Assistant Professor and Lecturer of Petroleum and Mining Engineering ',
                    link: '#'
                },
                {
                    time: Date.now(),
                    title: 'List of Selected Candidates for the post of Assistant Professor and Lecturer of Petroleum and Mining Engineering ',
                    link: '#'
                }
            ]
        }
    }
}
</script>

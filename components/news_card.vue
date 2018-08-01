<template>
    <div class="ncard">
        <div class="ncard__img">
            <img :src="src" alt="" class="ncard__img--img">
        </div>
        <div class="ncard__content">
            <span class="ncard__content--heading"> {{ heading }} </span> 
            <span class="ncard__content--time">  
                <span class="ncard__content--time-w">
                    <span class="ncard__content--time-i">
                        <i class="fas fa-clock"></i>
                    </span>
                     {{ time |  moment("h:mm A") }} 
                </span> 
                <span class="ncard__content--time-w">
                    <span class="ncard__content--time-i">
                        <i class="fas fa-calendar-alt"></i>
                    </span>
                     {{ time |  moment("MMMM Do, YYYY") }}
                </span>  
            </span>
            
            <span class="ncard__content--des">Exercitation sint ullamco qui laboris Lorem aliqua occaecat fugiat deserunt anim iras ipsum ea consequat aliquip...</span>
            <div class="d-flex justify-content-between ncard__content--link">
                <nuxt-link class="" :to="link">read full report</nuxt-link>
                <nuxt-link class="" :to="'/#'">
                    <span class="ncard__content--time-i">
                        <i class="fas fa-external-link-alt"></i>
                    </span> 
                    read all news
                </nuxt-link>
            </div> 
        </div>
    </div>
</template>

<script>
import moment from 'vue-moment'
export default {
    props: ['src', 'time', 'heading', 'link'],
    mounted() { 
    }
}
</script>

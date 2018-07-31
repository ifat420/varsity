<template>
    <div class="ncard">
        <div class="ncard__img">
            <img :src="src" alt="" class="ncard__img--img">
        </div>
        <div class="ncard__content">
            <span class="ncard__content--time"> {{ time |  moment("calendar") }} </span>
            <span class="ncard__content--heading"> {{ heading }} </span> 
            <!-- <nuxt-link class="ncard__content--link" :to="link">continue reading</nuxt-link> -->
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

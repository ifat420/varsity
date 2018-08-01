<template>
  <section class="">
    <app-hero/>
    <div class="container-fluid">
    <div class="row mt-5">
        <div class="newswrapper col-8">
            <app-news/>
            <app-workshop/>
        </div>
        <div class="col-4">
            <app-notice/>
        </div>
    </div>
    </div> 
    <app-overview/>
    <app-count/>
    <app-gallery/> 
  </section>
</template>

<script> 
import hero from '~/components/home_hero'
import news from '~/components/home_news'
import notice from '~/components/home_notice_board'
import workshop from '~/components/home_workshop'
import gallery from '~/components/home_gallery'
import overview from '~/components/home_overview'
import count from '~/components/home_count'
export default {
    layout: 'just',
    components: {
        'app-hero': hero,
        'app-news': news,
        'app-notice': notice,
        'app-workshop': workshop,
        'app-gallery': gallery,
        'app-overview': overview,
        'app-count': count
    },
    created() {
        console.log(this);
    }
}
</script>

 
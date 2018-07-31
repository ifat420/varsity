<template>
  <section class="">
     <app-hero/>
     <div class="container-fluid">
        <div class="row mt-5">
            <div class="section col-8">
                <app-news/>
                <app-workshop/>
            </div>
            <div class="col-4">
                <app-notice/>
            </div>
        </div>
     </div> 
  </section>
</template>

<script> 
import hero from '~/components/home_hero'
import news from '~/components/home_news'
import notice from '~/components/home_notice_board'
import workshop from '~/components/home_workshop'
export default {
    layout: 'just',
    components: {
        'app-hero': hero,
        'app-news': news,
        'app-notice': notice,
        'app-workshop': workshop,
    },
    created() {
        console.log(this);
    }
}
</script>

 
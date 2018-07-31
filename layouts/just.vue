<template>
    <div>
        <app-header/>
        <nuxt/>
        <app-footer/>
    </div>
</template>


<script>
import header from '~/components/home_header'
import footer from '~/components/home_footer' 
export default {
    components: {
        'app-header': header,
        'app-footer': footer,
    }
}
</script>

<style lang="scss">
@import '~/assets/styles/main.scss';
</style>

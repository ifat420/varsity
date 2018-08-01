<template>
    <div class="container-fluid p-0">
        <div class="row no-gutters">
            <div class="home-gallery-wrapper d-flex" > 
                <div class="home-gallery" v-for="(i, k) in 4" :key="k">
                    <img :src="imgs[k]" alt="" class="home-gallery__img">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            imgs: [
                '/1.jpg',
                '/07.jpg',
                '/03.jpg',
                '/08.jpg', 
            ]
        }
    }
}
</script>

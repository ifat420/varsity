<template> 
    <div class="container-fluid p-0">
        <div class="row no-gutters overview-wrapper">
            <div class="col-1">  
                <span class="overview__side">discover jessore university of science and technology</span>
            </div>
            <div class="col-3">
                <div class="overview__img">
                    <img src="/22.jpg" alt="" class="overview__img--img">
                </div>
            </div>
            <div class="col-7 offset-1 d-flex flex-column justify-content-center">
                <div class="overview">
                    <span class="overview__title">A brief overview</span>
                    <span class="overview__text">
                        {{ overview }}
                    </span>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            overview: ''
        }
    },
    created() {
        this.overview = 'Established in 2007, Jessore University of Science and Technology is a non-profit public higher education institution located in the the suburban setting of the large city of Jessore (population range of 1,000,000-5,000,000 inhabitants). Officially accredited and/or recognized by the University Grants Commission of Bangladesh, Jessore University of Science and Technology (JUST) is a very small (uniRank enrollment range: 500-999 students) coeducational higher education institution. Jessore University of Science and Technology (JUST) offers courses and programs leading to officially recognized higher education degrees such as pre-bachelor degrees (i.e. certificates, diplomas, associate or foundation degrees), bachelor degrees, master degrees, doctorate degrees in several areas of study. See the uniRank course levels and areas of studies matrix below for further details.'
    }
}
</script>

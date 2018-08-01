<template>
    <div class="container-fluid footer">
        <div class="row">
            <div class="col footer__social d-flex justify-content-start align-items-center">
                <h3>follow us</h3>
                <div class="footer__social--links">
                    <a href="#">
                        <i class="fab fa-facebook fa-1x"></i>
                    </a>
                    <a href="#">
                        <i class="fab fa-google-plus fa-1x"></i>
                    </a>
                    <a href="#">
                        <i class="fab fa-youtube fa-1x"></i>
                    </a>
                    <a href="#">
                        <i class="fab fa-twitter fa-1x"></i>
                    </a>
                </div>
            </div>
        </div>
        <div class="row footer__body">
            <div class="col-3">
                <div class="footer__info">
                    <img class="footer__info--img" src="/just.png" alt="">
                    <span class="footer__info--title">Jessore University of Science and Technology, Jessore – 7408</span>
                    <div class="footer__info--address">  
                        <strong>Tel:</strong> +880-421-61097, 61098, 62020, 62030, 62080, 63270, 63280 <br>
                        <strong>Fax:</strong>: 0421-61199, 0421-62238 <br>
                        <strong>Web:</strong>: www.just.edu.bd <br>
                        <strong>Email:</strong> vc@just.edu.bd, registrar@just.edu.bd <br>
                    </div>
                </div>
            </div>
            <div class="col-3 footer__list">
                
                <ul class="">
                    <span class="footer__list--header">Faculties</span>
                    <li v-for="(l, i) in faculties" :key="i" class="footer__list--item">
                        <nuxt-link :to="l.path">{{ l.title }}</nuxt-link>
                    </li>
                </ul>
            </div>
            <div class="col-3 footer__list">
                
                <ul class="">
                    <span class="footer__list--header">quick links</span>
                    <li v-for="(l, i) in quick" :key="i" class="footer__list--item">
                        <nuxt-link :to="l.path">{{ l.title }}</nuxt-link>
                    </li>
                </ul>
            </div>
            
            <div class="col-3 footer__list">
                <ul class="">
                    <span class="footer__list--header">important links</span>
                    <li v-for="(l, i) in ilinks" :key="i" class="footer__list--item">
                        <nuxt-link :to="l.path">{{ l.title }}</nuxt-link>
                    </li>
                </ul>
            </div>
            
        </div> 
        <div class="row footer__copywrite">
            <div class="col text-center">
                <span>© Jessore University of Science and Technology 2018</span>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            ilinks: [
                {
                    path: '#',
                    title: 'HEQEP'
                },
                {
                    path: '#',
                    title: 'Academic Calender'
                },
                {
                    path: '#',
                    title: 'Phonebook'
                },
                {
                    path: '#',
                    title: 'Bus Schedule'
                },
                {
                    path: '#',
                    title: 'Holiday Calendar 2018'
                },
                {
                    path: '#',
                    title: 'Committees and Working Groups'
                },
                {
                    path: '#',
                    title: 'Convocation'
                },
                {
                    path: '#',
                    title: 'Web Team and email Requests and Contacts'
                },
                {
                    path: '#',
                    title: 'Guest accommodation and Rest house booking information (Dhaka and in Campus)'
                },
                {
                    path: '#',
                    title: 'সমাচার'
                },
            ],
            faculties: [
                {
                    path: '#',
                    title: 'Faculty of Engineering and Technology'
                },
                {
                    path: '#',
                    title: 'Faculty of Biological Science and Technology'
                },
                {
                    path: '#',
                    title: 'Faculty of Applied Science and Technology'
                },
                {
                    path: '#',
                    title: 'Faculty of Science'
                },
                {
                    path: '#',
                    title: 'Faculty of Arts and Social Science'
                },
                {
                    path: '#',
                    title: 'Faulty of Business Studies'
                },
                {
                    path: '#',
                    title: 'Faculty of Health Science'
                } 
            ],
            quick: [
                {
                    path: '#',
                    title: 'Research'
                },
                {
                    path: '#',
                    title: 'Library'
                },
                {
                    path: '#',
                    title: 'Career'
                },
                {
                    path: '#',
                    title: 'Tender'
                },
                {
                    path: '#',
                    title: 'Maps'
                },
                {
                    path: '#',
                    title: 'Contact'
                },
                {
                    path: '#',
                    title: 'Administrative offices'
                },
                {
                    path: '#',
                    title: 'News & Events'
                },
                {
                    path: '#',
                    title: 'Gallery'
                } 
            ],
            
        }
    }
}
</script>

<template>
    <div class="container-fluid">
        <div class="row header">
            <div class="col-4 header__logo">
                <nuxt-link to="/">
                    <img src="/just.png" alt="" class="header__logo--img">
                </nuxt-link> 
                <!-- <span class="header__logo--text">Jessore University<br>of Science and<br>Technology</span> -->
            </div>
            <div class="col-8 header__navigation">
                <div class="header__navigation--secondary d-flex justify-content-end">
                    <nav> 
                        <nuxt-link v-for="(link, i) in sNav" :key="i" :to="link.path"> {{ link.title }} </nuxt-link>
                    </nav>
                </div>
                <div class="header__navigation--primary d-flex justify-content-end">
                    <nav class="navigation">
                        <ul class="navigation__list">
                            <li class="navigation__list--item" v-for="(nav, i) in pNav" :key="i"> 
                                <a href="#">
                                    {{ nav.name }}
                                    <i class="fas fa-angle-down ml-2"></i>
                                </a>
                                
                                <ul v-if="nav.links.length" class="navigation__list--item__sublist">
                                    <li class="navigation__list--item__sublist--item" v-for="(sub, k) in nav.links" :key="k">
                                        
                                        <nuxt-link :to="sub.path" >
                                            {{ sub.title }}  
                                        </nuxt-link> 
                                        
                                    </li>
                                </ul>
                            </li>
                        </ul>
                    </nav>
                </div>
            </div>
        </div>
    </div>
    
</template>

<script>
export default {
    data() {
        return {
            sNav: [
                {
                    path: '/research',
                    title: 'research'
                },
                {
                    path: '/career',
                    title: 'career'
                },
                {
                    path: '/academics/library',
                    title: 'library'
                },
                {
                    path: '/tender',
                    title: 'tender'
                }, 
                {
                    path: '/contact',
                    title: 'contact'
                },
                {
                    path: '/web-portal',
                    title: 'web portal'
                },
                {
                    path: '/webmail',
                    title: 'webmail'
                } 
            ],
            pNav: [
                {
                    name: 'discover just',
                    links: [
                        {
                            path: '/discover/just',
                            title: 'just at a glance'
                        },
                        {
                            path: '/discover/life',
                            title: 'life of just'
                        },
                        {
                            path: '/discover/halls',
                            title: 'student halls'
                        },
                        {
                            path: '/discover/journal-conferences',
                            title: 'journal and conferences'
                        },
                        {
                            path: '/discover/maps',
                            title: 'maps'
                        },
                    ]
                },
                {
                    name: 'admissions',
                    links: [
                        {
                            path: '/admissions/undergraduate',
                            title: 'undergraduate'
                        },
                        {
                            path: '/admissions/post-graduate',
                            title: 'post graduate'
                        },
                        {
                            path: '/admissions/diploma',
                            title: 'diploma'
                        },
                        {
                            path: '/admissions/foreign-students',
                            title: 'foreign students'
                        }  
                    ]
                },
                {
                    name: 'academics',
                    links: [
                        {
                            path: '/academics/institutes',
                            title: 'institutes'
                        },
                        {
                            path: '/academics/faculties',
                            title: 'faculties'
                        },
                        {
                            path: '/academics/library',
                            title: 'library'
                        },
                        {
                            path: '/academics/calender',
                            title: 'academic calender'
                        }  
                    ]
                },
                {
                    name: 'administrations',
                    links: [
                        {
                            path: '/administrations/offices',
                            title: 'administrative offices'
                        },
                        {
                            path: '/administrations/committees-and-working-group',
                            title: 'committees and working group'
                        },
                        {
                            path: '/administrations/authority',
                            title: 'authority'
                        } 
                    ]
                }
            ]
        }
    }
}
</script>

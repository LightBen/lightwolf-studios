<template>
    <transition name="pageTransition">
        <section id="projects">
            <div class="container-content">
                <p>Welcome to LightWolf Studios, creation of web apps. I am Benjamin Meir Khalifa, and I hope you will enjoy my portfolio. I am here to design and develop websites with the latest design trends and technologies.</p>
            </div>
            <h2 class="h2">Spotlight projects</h2>
            <div class="container-content">
                <div id="containerProjects" class="container-projects-general container-projects">
                    <a :href="project.link" target="_blank" class="project-item" :class="project.class" v-for="project in projects">
                        <div class="project-content">
                            <div class="project-name">{{ project.name }}</div>
                        </div>
                    </a>
                </div>
            </div>
            <h2 class="h2">We worked for them</h2>
            <div class="container-content">
                <div id="containerBrands" class="container-projects-general container-brands">
                    <div class="project-item" v-for="project in brands">
                        <div class="brand-logo" :class="project.class"></div>
                    </div>
                </div>
            </div>
            <h2 class="h2">Older projects</h2>
            <div class="container-content">
                <div id="containerProjectsPrev" class="container-projects-general container-projects-prev">
                    <a :href="project.link" target="_blank" class="project-item" :class="project.class" v-for="project in projectsPrev">
                        <div class="project-content">
                            <div class="project-name">{{ project.name }}</div>
                        </div>
                    </a>
                </div>
            </div>
            <h3 class="h3">With no preview anymore</h3>
            <div class="container-content">
                <div id="containerProjectsOld" class="container-projects-general container-projects-old">
                    <div class="project-item" :class="project.class" v-for="project in projectsOld">
                        <div class="project-content">
                            <div class="project-name">{{ project.name }}</div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </transition>
</template>

<script>
    export default {
        name: 'Projects',
        data() {
            return {
                projects: [
                    {
                        class: 'cm',
                        name: 'Constantine Minhagim',
                        link: 'http://constantine-minhagim.com',
                        desc: 'Constantine (Algeria) Jews traditions',
                        date: '2018',
                        tags: '#wordpress'
                    },
                    {
                        class: 'days',
                        name: '7 Days',
                        link: 'https://bereshit7days.web.app',
                        desc: '7 days of the Creation',
                        date: '2018',
                        tags: '#svg #animation #pwa #fromScratch'
                    },
                    {
                        class: 'mps',
                        name: 'My Perek Shira (early demo)',
                        link: 'https://my-perek-shira.web.app',
                        desc: 'Ancient Jewish text',
                        date: '2018',
                        tags: '#react #pwa'
                    },
                    {
                        class: 'commlife',
                        name: 'CommLife Solutions',
                        link: 'http://commlifesolutions.com',
                        desc: 'New technology for emergency',
                        date: '2017',
                        tags: '#wordpress'
                    },
                    {
                        class: 'sku',
                        name: 'Shaarey Kedusha',
                        link: 'http://new.sku26.com',
                        desc: 'Torah',
                        date: '2017',
                        tags: '#wordpress #youtubeApi'
                    },
                    {
                        class: 'lws-prev',
                        name: 'LightWolf Studios',
                        link: 'https://lws-prev.firebaseapp.com/lws-prev',
                        desc: 'Our previous portfolio',
                        date: '2014',
                        tags: '#fromScratch'
                    }
                ],
                brands: [
                    {
                        class: 'stanley',
                        name: 'Stanley',
                    },
                    {
                        class: 'tsystems',
                        name: 'T-Systems'
                    },
                    {
                        class: 'altria',
                        name: 'Altria'
                    },
                    {
                        class: 'numark',
                        name: 'Numark Innovations'
                    },
                    {
                        class: 'one',
                        name: '1One'
                    },
                    {
                        class: 'ashkelon-college',
                        name: 'Ashkelon College'
                    },
                    {
                        class: 'hdbt',
                        name: 'HDBT'
                    },
                    {
                        class: 'nice',
                        name: 'NICE'
                    },
                    {
                        class: 'panaya',
                        name: 'Panaya'
                    },
                    {
                        class: 'docomotion',
                        name: 'Docomotion'
                    },
                    {
                        class: 'credorax',
                        name: 'Credorax'
                    },
                    {
                        class: 'exlibris',
                        name: 'Ex Libris'
                    },
                    {
                        class: 'ipline',
                        name: 'IPLine'
                    },
                    {
                        class: 'valens',
                        name: 'Valens'
                    },
                    {
                        class: 'balink',
                        name: 'BA Link'
                    },
                ],
                projectsPrev: [
                    {
                        class: 'tekken-israel',
                        name: 'Tekken Israel',
                        link: 'http://tekken-israel.com',
                        desc: 'Video game community',
                        date: '2015',
                        tags: '#wordpress'
                    },
                    {
                        class: 'starlight',
                        name: 'Starlight',
                        link: 'http://starlight-zappings.com',
                        desc: 'Band\'s website',
                        date: '2008',
                        tags: '#fromScratch'
                    },
                    {
                        class: 'tlr',
                        name: 'Tekken Light Resurrection',
                        link: 'https://lws-prev.firebaseapp.com/tlr',
                        desc: 'Video games (Tekken) fan website',
                        date: '2007',
                        tags: '#fromScratch #tables #emotion #history'
                    }
                ],
                projectsOld: [
                    {
                        class: 'mt',
                        name: 'MarkTen',
                        link: 'https://markten.com',
                        desc: 'E-cigarettes',
                        date: '2018',
                        tags: '#ecommerce #magento'
                    },
                    {
                        class: 'gs',
                        name: 'Green Smoke',
                        link: 'https://www.greensmoke.com',
                        desc: 'E-cigarettes',
                        date: '2015-2018',
                        tags: '#ecommerce #magento'
                    },
                    {
                        class: 'ct',
                        name: 'Constantine Tefilot',
                        desc: 'Constantine (Algeria) Jews Liturgy',
                        date: '2016',
                        tags: '#wordpress'
                    },
                    {
                        class: 'mt-v1',
                        name: 'MarkTen v1',
                        desc: 'E-cigarettes',
                        date: '2015-2018',
                        tags: '#ecommerce #magento'
                    },
                    {
                        class: 'leoben',
                        name: 'Leron & Ben',
                        desc: 'Wedding website',
                        date: '2013',
                        tags: '#wordpress'
                    },
                    {
                        class: 'lbd',
                        name: 'LightBen\'s Design',
                        desc: 'Web design portfolio',
                        date: '2011',
                        tags: '#fromScratch'
                    },
                    {
                        class: 'naale',
                        name: 'Naale Tsion',
                        desc: 'French High school in Israel',
                        date: '2012',
                        tags: '#wordpress'
                    },
                    {
                        class: 'sabao',
                        name: 'SabaO',
                        desc: 'Home made soap',
                        date: '2011',
                        tags: "#ecommerce"
                    },
                    {
                        class: 'zappings',
                        name: 'Les Zappings',
                        link: 'http://www.spectacle-enfant-zapping.fr',
                        desc: 'Animation group for children',
                        date: '2008',
                        tags: '#fromScratch'
                    }
                ]
            }
        }
    }
</script>

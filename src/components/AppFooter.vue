<template>
    <footer>
        <div class="container">
            <div class="footer_lists">
                <AppFooterList 
                    title="DC COMICS" 
                    :links="links1"
                />
                <AppFooterList 
                    title="SHOP" 
                    :links="links2"
                />
                <AppFooterList 
                    title="DC" 
                    :links="links3"
                />
                <AppFooterList 
                    title="SITES" 
                    :links="links4"
                />
            </div>
            <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>
    </footer>
</template>

<script>
import AppFooterList from '@/components/AppFooterList.vue'

export default {
    name : 'AppFooter',
    components : {
        AppFooterList,
    },
    data () {
        return {
            links1 : [
                {
                    'name' : 'Characters',
                    'href' : '#'
                },
                {
                    'name' : 'Comics',
                    'href' : '#'
                },
                {
                    'name' : 'Movies',
                    'href' : '#'
                },
                {
                    'name' : 'TV',
                    'href' : '#'
                },
                {
                    'name' : 'Games',
                    'href' : '#'
                },
                {
                    'name' : 'Videos',
                    'href' : '#'
                },
                {
                    'name' : 'News',
                    'href' : '#'
                }
            ],
            links2 : [
                {
                    'name' : 'Shop DC',
                    'href' : '#'
                },
                {
                    'name' : 'Shop DC Collectibles',
                    'href' : '#'
                }
            ],
            links3 : [
                {
                    'name' : 'Terms Of Use',
                    'href' : '#'
                },
                {
                    'name' : 'Privacy policy(New)',
                    'href' : '#'
                },
                {
                    'name' : 'Ad Choices',
                    'href' : '#'
                },
                {
                    'name' : 'Advertaising',
                    'href' : '#'
                },
                {
                    'name' : 'Jobs',
                    'href' : '#'
                },
                {
                    'name' : 'Subscriptions',
                    'href' : '#'
                },
                {
                    'name' : 'Talent Workshops',
                    'href' : '#'
                },
                {
                    'name' : 'CPSC Certificates',
                    'href' : '#'
                },
                {
                    'name' : 'Ratings',
                    'href' : '#'
                },
                {
                    'name' : 'Shop Help',
                    'href' : '#'
                },
                {
                    'name' : 'Contact Us',
                    'href' : '#'
                }
            ],
            links4 : [
                {
                    'name' : 'DC',
                    'href' : '#'
                },
                {
                    'name' : 'MAD Magazine',
                    'href' : '#'
                },
                {
                    'name' : 'DC Kids',
                    'href' : '#'
                },
                {
                    'name' : 'DC Universe',
                    'href' : '#'
                },
                {
                    'name' : 'DC PowerVisa',
                    'href' : '#'
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss" >
footer {
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    height: 380px;

    .container {
        display: flex;
        justify-content: space-between;

        .footer_lists {
            display: flex;
            flex-wrap: wrap;
            flex-direction: column;
            padding: 30px 0;
        }
        
        img {
            width: 45%;
            aspect-ratio: 1;
            object-fit: cover;
            object-position: center;
        }
    }
}
</style>
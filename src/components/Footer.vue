<template>
  <footer>
        <div class="footer_lists">
            <span>
                <List 
                    title="DC COMICS" 
                    :links="links1"
                />
                <List 
                    title="SHOP" 
                    :links="links2"
                />
            </span>
            <List 
                title="DC" 
                :links="links3"
            />
            <List 
                title="SITES" 
                :links="links4"
            />
        </div>
        <div class="prova">
            <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>
  </footer>
</template>

<script>
import List from '@/components/List.vue'

export default {
    name : 'Footer',
    components : {
        List,
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
    display: flex;
    justify-content: space-between;
    height: 380px;

    .footer_lists {
        height: 100%;
        display: flex;
        flex-wrap: 1;
        flex-direction: row;
        padding: 30px;
    }

    .prova  {
        height: 100%;

        img {
            object-fit: cover;
            height: 120%;
        }
    }
}
</style>
<template>
    <section>
        <div class="container">
            <a class="sign-up" href="#">
                SIGN-UP NOW!
            </a>
            <ul>
                <li v-for="social, i in socials" :key="i">
                    <a :href="social.href">
                        <!-- <img :src="require(`${social.img}`)" alt=""> -->
                        <!-- <img src="../assets/img/footer-facebook.png" alt=""> -->
                    </a>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
export default {
    name : 'AppFooterContacts',
    data() {
        return {
            socials : [
                {
                    'img' : '../assets/img/footer-facebook.png',
                    'href' : '#'
                },
                {
                    'img' : '../assets/img/footer-twitter.png',
                    'href' : '#'
                },
                {
                    'img' : '../assets/img/footer-youtube.png',
                    'href' : '#'
                },
                {
                    'img' : '../assets/img/footer-pinterest.png',
                    'href' : '#'
                },
                {
                    'img' : '../assets/img/footer-periscope.png',
                    'href' : '#'
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss" >
section {
    background-color: #303030;
    
    .container {
        padding: 20px 0;
        display: flex;
        justify-content: space-between;
        align-items: center;
    
        .sign-up {
            display: inline-block;
            border: 2px solid #3183fc;
            color: white;
            padding: 15px;
            text-decoration: none;
        }

        ul {
            list-style: none;
            display: flex;
        }
    }
}


</style>
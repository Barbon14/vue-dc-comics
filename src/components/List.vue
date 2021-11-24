<template>
    <div>
        <h4>
            {{ title }}
        </h4>
        <ul>
            <li v-for="link, i in links" :key="i">
                    <a :href="link.href">
                        {{ link.name }}
                    </a>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name : 'List',
    props : {
        title : String,
        links : Array
    },
}
</script>

<style scoped lang="scss" >
h4 {
    color: white;
    margin-bottom: 10px;
}

ul {
    margin-bottom: 15px;
    margin-right: 25px;

    li {
        list-style: none;
        margin: 5px 0;

        a {
            text-decoration: none;
            color: #959595;
        }
    }
}
</style>
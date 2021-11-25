<template>
    <div class="card">
        <img :src="info.thumb" :alt="info.series">
        <h4>
            {{ info.series }}
        </h4>
    </div>
</template>

<script>
export default {
    name : 'Card',
    props : {
        info : Object
    },
}
</script>

<style scoped lang="scss" >
.card {
    width: calc(100% / 6);
    padding: 20px;

    img {
        width: 100%;
        aspect-ratio: 1;
        object-fit: cover;
        object-position: top;
    }

    h4 {
        margin: 10px 0;
        color: white;
    }
}
</style>
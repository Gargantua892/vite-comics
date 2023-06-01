<template>
    <div class="comic-card">
        <img :src="details.thumb" alt="">
        <h5 class="mt-2">{{details.series}}</h5>
    </div>
</template>

<script>
export default {
    props: {
        details: Object,
    }
}
</script>

<style lang="scss">

.comic-card{
    width: calc((100% / 6) - 16px );
    color: #fff;
    img{
        width: 100%;
        height: 200px;
        object-fit: cover;

    }
}

</style>

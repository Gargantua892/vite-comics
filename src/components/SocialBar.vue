<template>
    <div>
        <div class="container d-flex justify-content-between py-4">
            <div class="button button-linear">Sign-up Now</div>
            <div class="social-container d-flex align-items-center gap-2">
                <h5>follow us</h5>
                <img src="../assets/img/footer-facebook.png" alt="">
                <img src="../assets/img/footer-periscope.png" alt="">
                <img src="../assets/img/footer-pinterest.png" alt="">
                <img src="../assets/img/footer-twitter.png" alt="">
                <img src="../assets/img/footer-youtube.png" alt="">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data () {
        return {
           
        }
    },
    methods: {

    },
}
</script>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;

h5{
    margin: 0px;
    color: $primary;
}

*{
    background-color: #303030;
    color: #fff;
}

.button-linear{
    border: 2px solid $primary;
}


</style>
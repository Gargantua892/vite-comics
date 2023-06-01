<template>
    <div>
        <div class="service-bar py-4">
            <div class="container">
                <div class="justify-content-center d-flex justify-content-around flex-wrap">
                    <div v-for="service in services" class="d-flex align-items-center gap-2">
                        <img :src="getImagePath(`../assets/img/${service.img}`)" alt="">
                        <h5>{{service.text}}</h5>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data () {
        return {
            services: [
                {
                    img: "buy-comics-digital-comics.png",
                    text: "Digital Comics"
                },
                {
                    img: "buy-comics-merchandise.png",
                    text: "DC Merchandise"
                },
                {
                    img: "buy-comics-subscriptions.png",
                    text: "Subscription"
                },
                {
                    img: "buy-comics-shop-locator.png",
                    text: "Comic shop locator"
                },
                {
                    img: "buy-dc-power-visa.svg",
                    text: "DC power visa"
                },
            ]
        }
    },
    methods: {
        getImagePath: function(imgPath){
            return new URL(imgPath, import.meta.url).href;
        }
    },
}
</script>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;
    .service-bar{
        background-color: $primary;
        color: #fff;

        img{
            width: 36px;
        }

        h5{
            font-size: 14px;
            text-transform: uppercase;
            margin: 0px;
        }
    }
</style>
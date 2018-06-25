<template>
    <div :class="cname">
        <swiper :options="swiperOption" :not-next-tick="swiperOption.notNextTick">
            <swiper-slide v-for="item in swiperSlides" :key="item.href">
                <router-link :to="item.href">
                    <img :src="item.src" alt="">
                </router-link>
            </swiper-slide>
            <div class="swiper-pagination" slot="pagination"></div>
        </swiper>
    </div>
</template>

<script type="text/ecmascript-6">
    import { swiper, swiperSlide } from 'vue-awesome-swiper'
    export default {
        name: "Slider",
        props: {
            cname: String,
            swiperOption: {
                type: Object,
                default () {
                    return {
                        autoplay: true,
                        loop: true,
                        pagination: {
                            el: '.swiper-pagination',
                        },
                        autoplay:{
                            disableOnInteraction: false
                        },
                        notNextTick: false,
                    }
                }
            },
            swiperSlides: Array
        },
        components: {
            swiper,
            swiperSlide
        }
    }
</script>

<style lang="scss">
    @import '~swiper/dist/css/swiper.css';
</style>
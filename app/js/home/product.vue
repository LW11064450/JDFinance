<template>
    <Panel title="新品推荐" :class="$style.panel">
        <div :class="$style.panel_content">
            <Slider :swiperSlides="swiperSlides" :swiperOption="swiperOption" cname="product-slider"></Slider>
        </div>
        <div :class="$style.more">更多尖货></div>
    </Panel>
</template>

<script type="text/ecmascript-6">
    import Panel from '../core/panel'
    import Slider from "../core/slider"
    export default {
        name: "",
        data () {
            return {
                swiperSlides: [
                    {
                        href: "/",
                        src: "//img12.360buyimg.com/jrpmobile/jfs/t13963/267/2355123229/48850/254f797a/5a3c59aeN9cb550f6.jpg?width=335&height=421",
                    }, {
                        href: "/",
                        src: "//img12.360buyimg.com/jrpmobile/jfs/t13021/306/1996997425/21953/bda69db3/5a2f6a17N9da099b1.jpg?width=335&height=421",
                    }, {
                        href: "/",
                        src: "//img12.360buyimg.com/jrpmobile/jfs/t14125/310/1997192193/46667/3c910f8b/5a2f6a36Nad95b650.jpg?width=335&height=421",
                    }, {
                        href: "/",
                        src: "//img12.360buyimg.com/jrpmobile/jfs/t15784/188/381232069/39444/8878571d/5a2f6a4aNbd5a574c.jpg?width=335&height=421",
                    }
                ],
                swiperOption: {
                    slidesPerView: 2.3,
                    spaceBetween: 30,
                    freeMode: true,
                }
            }
        },
        components: {
            Panel,
            Slider
        }
    }
</script>

<style lang="scss" type="text/scss">
    .product-slider{
        .swiper-container{
            box-sizing: border-box;
            padding: 0 24px;
            .swiper-slide{
                a{
                    display: inline-block;
                    img{
                        display: block;
                        width: 100%;
                        height: 314px;
                        border: 1px solid #fafafa;

                    }
                }
            }
        }
    }

</style>

<style lang="scss" type="text/scss" module>
    .panel{
        position: relative;
        padding-bottom: 40px;
        .more{
            position: absolute;
            right:20px;
            top: 42px;
            font-size: 28px;
            color: #999999;
        }
    }
</style>
<template>
    <Slider :swiperSlides="swiperSlides" :cname="$style.slider"></Slider>
</template>

<script type="text/ecmascript-6">
    import Slider from '../core/slider'
    export default {
        name: "",
        data () {
            return {
                swiperSlides: [
                    {
                        href: "/",
                        src: "//img12.360buyimg.com/jrpmobile/jfs/t11149/181/856008463/68797/dc303e9/59f97baeN3cdae084.jpg?width=750&height=400",
                    }, {
                        href: "/",
                        src: "//img12.360buyimg.com/jrpmobile/jfs/t9994/205/2575467053/189117/125e7b05/59f97c36N7599be57.png?width=750&height=400",
                    }
                ]
            }
        },
        components: {
            Slider
        }
    }
</script>

<style lang="scss" type="text/scss" module>
    .slider{
        width: 100%;
        height: 0;
        padding-bottom: 53.3333333%;
        margin-top: 120px;
        overflow: hidden;
        a{
            display: block;
            img{
                width: 100%;
            }
        }
    }
</style>
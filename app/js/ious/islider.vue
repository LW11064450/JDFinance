<template>
    <Slider :swiperSlides="swiperSlides" :cname="$style.slider"></Slider>
</template>

<script type="text/ecmascript-6">
    import Slider from '../core/slider'
    export default {
        name: "",
        data () {
            return {
                swiperSlides: [{
                    href: "ious",
                    src: "//img12.360buyimg.com/jrpmobile/jfs/t8491/303/504628479/60643/100648de/59a94358N92475fca.jpg?width=750&height=320",
                }, {
                    href: "home",
                    src: "//img12.360buyimg.com/jrpmobile/jfs/t8437/321/1758527686/40952/f66d552f/59bf1f41N50d846f9.jpg?width=750&height=320",
                }],
            }
        },
        components: {
            Slider
        }
    }
</script>

<style lang="scss" type="text/scss" module>
    .slider{
        height: 0;
        padding-bottom: 42.667%;
        margin-top: 120px;
        overflow: hidden;
        img{
            width: 100%;
        }
    }
</style>
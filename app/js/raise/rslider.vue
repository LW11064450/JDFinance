<template>
    <Panel title="金融头条" :cname="$style.panel">
        <div :class="$style.slider">
            <swiper :options="options">
                <swiper-slide>百万白条券免费送，速来领取！！ <em>></em> </swiper-slide>
                <swiper-slide>签到领流量，1元500M！<em>></em> </swiper-slide>
            </swiper>
        </div>
    </Panel>
</template>

<script type="text/ecmascript-6">
    import Panel from '../core/panel'
    import { swiper, swiperSlide } from 'vue-awesome-swiper'
    export default {
        name: "",
        data () {
            return {
                options: {
                    direction: 'vertical',
                    autoplay: true,
                    loop: true,
                }
            }
        },
        components: {
            Panel,
            swiper,
            swiperSlide
        }
    }
</script>

<style lang="scss" type="text/scss">
    .swiper-container {
        height: 72px;
        .swiper-slide{
            font-family: PingFangSC-Medium;
            font-size: 28px;
            color: #333;
            em{
                color: #ddd;
                float: right;
                margin-right: 20px;
            }
        }
    }

</style>
<style lang="scss" type="text/scss" module>
    .panel{
        margin-top: 120px !important;
        h4{
            display: none;
        }
        .slider{
            height: 72px;
            line-height: 72px;
            padding-left: 178px;
            overflow: hidden;
            background: url(//m.jr.jd.com/spe/qyy/main/images/scroll_title_img.png) 0 8px no-repeat;
        }
    }
</style>
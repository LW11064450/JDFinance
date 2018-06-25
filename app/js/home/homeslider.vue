<template>
    <div class="slider-wrap">
        <slider :swiperSlides="swiperSlides" :cname="$style.slider"></slider>
        <div :class="$style.List">
            <ul :class="$style.list_wrap">
                <li :class="$style.list_item" v-for="item in enters" :key="item.img">
                    <router-link :to="item.href">
                        <img :src="item.src" :alt="item.title">
                        <h4>{{item.title}}</h4>
                    </router-link>
                </li>
            </ul>
        </div>
    </div>
</template>

<script type="text/ecmascript-6">
    import Slider from "../core/slider"
    export default {
        name: "",
        data () {
            return {
                swiperSlides: [
                    {
                        href: "/",
                        src: "https://img12.360buyimg.com/jrpmobile/jfs/t20422/12/1263160918/43632/2a39e361/5b23b5e2N29ae9036.jpg?width=750&height=320"
                    },{
                        href:"/",
                        src:"https://img12.360buyimg.com/jrpmobile/jfs/t21592/320/1276596164/54867/155e9c84/5b23b618N57820072.jpg?width=750&height=320"
                    },{
                        href:"/",
                        src:"https://img12.360buyimg.com/jrpmobile/jfs/t20362/86/1263465194/44494/211ed62f/5b23b633Ndaf4ecd6.jpg?width=750&height=320"
                    },{
                        href:"/",
                        src:"https://img12.360buyimg.com/jrpmobile/jfs/t21385/135/1201527515/55111/e89a9ff6/5b221ccbNd9ffa09f.jpg?width=750&height=320"
                    }
                ],
                enters: [
                    {
                        src:'https://img12.360buyimg.com/jrpmobile/jfs/t3991/64/2521945388/12110/93c0139/58d1e462Ncf294123.png?width=132&height=132',
                        href:'/',
                        title: '优惠券'
                    },{
                        src:'https://img12.360buyimg.com/jrpmobile/jfs/t5590/252/875247023/17343/946aa72c/59224650N0f7ffc92.png?width=132&height=132',
                        href:'/',
                        title: '领红包'
                    },{
                        src:'https://img12.360buyimg.com/jrpmobile/jfs/t4393/329/2180608902/13217/c88c0cec/58ec9dcdN1534e2d7.png?width=132&height=132',
                        href:'/',
                        title: '抢钢镚'
                    },{
                        src:'https://img12.360buyimg.com/jrpmobile/jfs/t5488/298/1036263348/12073/b4f4de97/590ac8e8Ne9def22e.png?width=135&height=135',
                        href:'/',
                        title: '白条提额'
                    }
                ]

            }

        },
        components:{
            Slider
        }
    }
</script>

<style lang="scss" type="text/scss" module>
    @import "../../css/element.scss";
    .slider{
        margin-top: 120px;
        height: 0;
        padding-bottom: 42.667%;
        overflow: hidden;
        a{
            display: block;
            img{
                width: 100%;
            }
        }
        .swiper-pagination-bullet{
            width: 12px;
            height: 12px;
        }

    }
    .list_wrap{
        @include list(row);
        background: #fff;
        padding-top: 40px;
        padding-bottom: 20px;
        justify-content: space-around;
        .list_item{
            text-align: center;
            img{
                display: inline-block;
                width: 90px;
                height: 90px;
            }
            h4{
                font-size: 26px;
                margin-top: 12px;
            }
        }
    }

</style>
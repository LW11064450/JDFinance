<template>
    <Panel title="每日签到" :class="$style.panel">
        <div :class="$style.content">
            <img src="//img12.360buyimg.com/jrpmobile/jfs/t3184/283/6032981290/37056/fa30c674/589bd5a2Nabdbbbd9.jpg?width=376&height=160" alt="">
            <img src="//img12.360buyimg.com/jrpmobile/jfs/t3298/196/6130416421/33755/a0536d3e/589bd5d4Nf32e7adc.jpg?width=374&height=160" alt="">
        </div>
    </Panel>
</template>

<script type="text/ecmascript-6">
    import Panel from '../core/panel'
    export default {
        name: "",
        components: {
            Panel
        }
    }
</script>

<style lang="scss" type="text/scss" module>
    @import "../../css/element";
    .panel{
        position: relative;
        &::after{
            content: '不抢白不抢';
            position: absolute;
            top: 0;
            right: 25px;
            height: 112px;
            line-height: 112px;
            font-size: 28px;
            color: #999;
        }
        .content{
            @include list(row);
            img{
                width: 320px;
                height: 136px;
            }
        }
    }

</style>
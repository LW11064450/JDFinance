<template>
    <Panel title="更多福利" :class="$style.panel">
        <div :class="$style.content">
            <img src="//img12.360buyimg.com/jrpmobile/jfs/t7456/56/1425209238/21928/f1fe492d/599cee57Naea99020.jpg?width=250&height=330" alt="">
            <img src="//img12.360buyimg.com/jrpmobile/jfs/t7894/126/1440046618/24763/5ce6a129/599cee04Ne77b3641.jpg?width=250&height=330" alt="">
            <img src="//img12.360buyimg.com/jrpmobile/jfs/t6385/103/1675552688/24265/91be4150/59549aedNa30670f7.jpg?width=250&height=330" alt="">
        </div>
    </Panel>
</template>

<script type="text/ecmascript-6">
    import Panel from "../core/panel.vue"
    export default {
        components: {
            Panel,
        },
    }
</script>

<style lang="scss" type="text/scss" module>
    @import "../../css/element";
    .panel{
        position: relative;
        .content{
            @include list(row);

            padding-bottom: 30px;
            img{
                flex: 1;
                height: 280px;
            }
        }
        &::after{
            content: '专享福利 >';
            position: absolute;
            top: 0;
            right: 25px;
            height: 112px;
            line-height: 112px;
            font-size: 28px;
            color: #999;
        }
    }

</style>
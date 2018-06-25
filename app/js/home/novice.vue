<template>
    <Panel title="新手特权" :cname="$style.panel">
        <div :class="$style.panel_content">
            <div :class="$style.panel_item">
                <h4>下载APP<span :class="$style.red">送888元礼包</span></h4>
                <p :class="$style.gray">新手专享</p>
                <img src="//img12.360buyimg.com/jrpmobile/jfs/t10384/155/1759179594/9776/185bd062/59e5f0ebNec4cf494.png?width=100&height=100" alt="">
            </div>
            <div :class="$style.panel_item">
                <ul :class="$style.item_wrap">
                    <li>
                        <div :class="$style.item_img">
                            <img src="//img12.360buyimg.com/jrpmobile/jfs/t4639/162/1782623297/60754/98ea03b4/58e60952N7fdb2b85.png?width=200&height=200" alt="">
                        </div>
                        <div :class="$style.item_info">
                            <h4 :class="$style.red">领128元新手礼包</h4>
                            <p :class="$style.gray">立即开通</p>
                        </div>
                    </li>
                    <li>
                        <div :class="$style.item_img">
                            <img src="//img12.360buyimg.com/jrpmobile/jfs/t4804/179/657713323/5908/66dce262/58e6095fNd3dc3f39.png?width=100&height=100" alt="">
                        </div>
                        <div :class="$style.item_info">
                            <h4>打白条<span :class="$style.red">享免息</span></h4>
                            <p :class="$style.gray">立即开通享豪礼</p>
                        </div>
                    </li>
                </ul>
            </div>
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
    @import "../../css/element.scss";
    .panel_content{
        @include list(row);
        .panel_item{
            width: 50%;
            box-sizing: border-box;
            &:first-child{
                text-align: center;
                padding: 32px 32px;
                border-right: 1px solid #ddd;
                img{
                    margin-top: 20px;
                }
            }
            h4{
                height: 40px;
                line-height: 40px;
                font-size: 26px;
                span{
                    vertical-align: baseline;
                }
            }
            p{
                margin-top: 6px;
            }
            .red{
                color: #f00;
            }
            .gray{
                color: #999;
                font-size: 24px;
            }
            .item_wrap{
                li{
                    height: 144px;
                    padding: 32px 28px;
                    box-sizing: border-box;
                    overflow: hidden;
                    .item_info{
                        float: left;
                        width: 184px;
                        h4{
                            white-space: nowrap;
                            text-overflow: ellipsis;
                            overflow: hidden;
                        }
                    }
                    .item_img{
                        float: right;
                        width: 80px;
                        height: 80px;
                        img{
                            width: 100%;
                        }
                    }
                    &:first-child{
                        border-bottom: 1px solid #ddd;
                    }
                }

            }
        }
    }
</style>
<template>
    <Panel title="理财精选">
        <div :class="$style.content">
            <div :class="$style.item">
                <img src="//img12.360buyimg.com/jrpmobile/jfs/t3670/58/543125556/2606/a65096b9/580d80afN63b1085a.png?width=76&height=76" alt="">
                <div :class="$style.info">
                    <h4>月度理财</h4>
                    <p>预期年化收益率4.50%</p>
                </div>
                <em>去赚钱 > </em>
            </div>
            <div :class="$style.item">
                <img src="//img12.360buyimg.com/jrpmobile/jfs/t3679/44/511862277/2728/c1c6b2bf/580d8189N6b6f8052.png?width=76&height=76" alt="">
                <div :class="$style.info">
                    <h4>季度理财</h4>
                    <p>历史年化回报率5.50%</p>
                </div>
                <em>去赚钱 > </em>
            </div>
            <div :class="$style.item">
                <img src="//img12.360buyimg.com/jrpmobile/jfs/t3331/69/580199498/3074/d5bb21c5/580d7f6cN7f35e596.png?width=76&height=76" alt="">
                <div :class="$style.info">
                    <h4>一年理财</h4>
                    <p>历史年化回报率5.80%</p>
                </div>
                <em>去赚钱 > </em>
            </div>
        </div>
    </Panel>
</template>

<script type="text/ecmascript-6">
    import Panel from "../core/panel"
    export default {
        name: "",
        components: {
            Panel
        }
    }
</script>

<style lang="scss" type="text/scss" module>
    @import "../../css/element";
    .content{
        .item{
            @include list(row);
            height: 140px;
            padding: 20px 30px;
            align-items: center;
            box-sizing: border-box;
            &::after{
                content: '';
                width: 100%;
                height: 0;
                margin-left: 140px;
                border-bottom: 1px solid #ddd;
            }
            &:last-child::after{
                border: none;
            }
            img{
                width: 88px;
                height: 88px;
                margin-right: 32px;
            }
            .info{
                flex: 1;
                font-size: 32px;
                line-height: 1.8;
                color: #333;
                p{
                    color: #ff3232;
                    font-size: 24px;
                    line-height: 1.1;
                    white-space: nowrap;
                    text-overflow: ellipsis;
                    overflow: hidden;
                }
            }
            em{
                color: #FF801A;
                font-size: 28px;
            }
        }

    }
</style>
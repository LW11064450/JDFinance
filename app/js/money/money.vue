<template>
    <Panel title="理财精选">
        <div :class="$style.panel_content">
            <dl :class="$style.panel_item" v-for="item in moneyData" :key="item.title">
                <dt>{{ item.title }}<span>{{ item.sub }}</span></dt>
                <dd>{{ item.rate }}</dd>
                <dd>{{ item.text }}</dd>
            </dl>
        </div>
    </Panel>
</template>

<script type="text/ecmascript-6">
    import Panel from "../core/panel"
    export default {
        name: "",
        data () {
            return {
                moneyData: [
                    {
                        title: "定期理财",
                        sub: "理财首选",
                        rate: "5.60%",
                        text: "历史年化回报率",
                    }, {
                        title: "小白理财",
                        sub: "理财首选",
                        rate: "4.22%",
                        text: "7日年化收益率",
                    }, {
                        title: "月月盈",
                        sub: "养老保障",
                        rate: "5%",
                        text: "七日年化收益率",
                    }, {
                        title: "小白基金",
                        sub: "天天赚钱",
                        rate: "4.27%",
                        text: "7日年化收益率",
                    }
                ]

            }
        },
        components: {
            Panel
        }
    }
</script>

<style lang="scss" type="text/scss" module>
    @import '../../css/element.scss';
    .panel_content{
        @include list(row);
        justify-content: space-around;
        &::after{
            content: '';
            position: relative;
            width: 100%;
            height: 0;
            border-bottom: 1px solid #eee;
            box-sizing: border-box;
            top: -208px;
        }
    }
    .panel_item{
        position: relative;
        width: 50%;
        padding: 34px 16px;
        box-sizing: border-box;
        &::after{
            content: '';
            position: absolute;
            width: 1px;
            height: 136px;
            top: 50%;
            right: 0;
            margin-top: -68px;
            border-right: 1px solid #eee;
        }
        &:nth-child(2n){
            &::after{
                border: 0;
            }
        }
        dt{
            font-size: 38px;
            line-height: 42px;
            color: #333;
            span{
                font-size: 22px;
                color: #ff5155;
                border: 1px solid #ff5155;
                padding: 0 8px;
                vertical-align: middle;
                margin-left: 4px;
            }
        }
        dd{
            &:nth-child(2){
                height: 58px;
                line-height: 58px;
                font-size: 44px;
                font-weight: 700;
                color: #ff5155;
                white-space: nowrap;
                text-overflow: ellipsis;
                overflow: hidden;
            }
            &:nth-child(3){
                font-size: 24px;
                height: 34px;
                line-height: 34px;
                color: #999;
                white-space: nowrap;
                text-overflow: ellipsis;
                overflow: hidden;
            }
        }
    }
</style>
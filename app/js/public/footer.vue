<template>
    <footer :class="[$style.footer,cname]">
        <ul :class="$style.content">
            <li :class="$style.help_center">
                <img src="//img12.360buyimg.com/jrpmobile/jfs/t2842/350/3035567089/14791/5f6ff93d/577cf395N31e76288.png?width=1125&height=252" alt="">
            </li>
            <li :class="$style.download_list">
                <div>
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t2971/333/1297567079/898/f2d2e00d/577dc28dNe5138337.png?width=108&height=108" alt="">
                    <p>客户端</p>
                </div>
                <div>
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t2824/256/2966087355/831/188bfa25/577cf3dcN18aadbf2.png?width=108&height=108" alt="">
                    <p>触屏版</p>
                </div>
                <div>
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t2920/282/1283157010/1040/23f1430b/577cf3e5N53f740b8.png?width=108&height=108" alt="">
                    <p>电脑版</p>
                </div>
            </li>
            <li>Copyright © 2004-2017 京东JD.com 版权所有</li>
            <li>投资有风险，购买需谨慎</li>
            <li>京东金融平台服务协议</li>
            <li>京东金融隐私政策</li>
        </ul>
    </footer>
</template>

<script type="text/ecmascript-6">
    export default {
        name: "",
        props: {
            cname: String
        }
    }
</script>

<style lang="scss" type="text/scss" module>
    @import "../../css/element.scss";
    .footer{
        margin-bottom: 100px;
        .content{
            li{
                color: #999;
                font-size: 24px;
                text-align: center;
                &.help_center {
                    width: 100%;
                    height: 0;
                    padding-bottom: 22.4%;
                    overflow: hidden;
                    img {
                        width: 100%;
                    }
                }
                &.download_list {
                    @include list(row);
                    height: 186px;
                    justify-content: space-around;
                    padding-top: 30px;
                    box-sizing: border-box;
                    p {
                        font-size: 26px;
                        text-align: center;
                        color: #999;
                        margin-top: 12px;
                        white-space: nowrap;
                        text-overflow: ellipsis;
                        overflow: hidden;
                    }
                    img {
                        display: inline-block;
                        width: 90px;
                        height: 90px;
                    }
                }
                &:nth-child(n+3){
                    padding: 24px 0;
                    height: 38px;
                    line-height: 38px;
                    border-top: 1px solid #ddd;
                }
            }
        }

    }
</style>
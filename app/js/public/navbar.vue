<template>
    <div :class="$style.navbar">
        <ul :class="$style.content">
            <li>
                <router-link to="/">
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t3451/188/644771475/2428/800d7cb7/580f2435Nbfaa8055.png?width=66&height=66" alt="">
                    <p>首页</p>
                </router-link>
            </li>
            <li>
                <router-link to="/money">
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t3811/55/345433999/2930/116d3dd1/580f1e25N028a1f2c.png?width=66&height=66" alt="">
                    <p>理财</p>
                </router-link>
            </li>
            <li>
                <router-link to="/ious"><img src="//img12.360buyimg.com/jrpmobile/jfs/t3343/179/621044750/1484/5af6b11a/580f50e4N005181d0.png?width=66&height=66" alt="">
                    <p>白条</p></router-link>
            </li>
            <li>
                <router-link to="/raise">
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t3604/98/635506544/2317/443d3a51/580f240aNbee3dcc4.png?width=66&height=66" alt="">
                    <p>众筹</p>
                </router-link>
            </li>
            <li>
                <img src="//img12.360buyimg.com/jrpmobile/jfs/t3340/68/639059082/2591/800e2d6b/580f51cdN4caf20b2.png?width=66&height=66" alt="">
                <p>我的</p>
            </li>
        </ul>
    </div>
</template>

<script type="text/ecmascript-6">
    export default {
        name: ""
    }
</script>

<style lang="scss" type="text/scss" module>
    @import "../../css/element.scss";
    .navbar{
        position: fixed;
        width: 100%;
        height: 100px;
        bottom: 0;
        left: 0;
        background-color: #fff;
        z-index: 2;
        .content{
            @include list(row);
            justify-content: space-around;
            text-align: center;
            li{
                img{
                    display: inline-block;
                    width: 44px;
                    height: 44px;
                    margin: 12px 0;
                }
                p{
                    font-size: 22px;
                    color: #656565;
                }
            }
        }
    }
</style>
<template>
    <div :class="$style.header">
        <div :class="$style.login_area">
            <span :class="$style.user_Login">注册 | 登陆</span>
        </div>
        <img :class="$style.header_logo" src="https://m.jr.jd.com/spe/qyy/main/images/jr-logo.png" alt="">
        <btn :class="$style.download_btn">APP下载</btn>
    </div>
</template>

<script type="text/ecmascript-6">
    import Btn from "../core/btn"
    export default {
        name: "",
        components: {
            Btn,
        }
    }
</script>

<style lang="scss" type="text/scss" module>
    .header{
        position: fixed;
        height: 100px;
        font-size: 32px;
        color: #666;
        background-color: #fff;
        top: 0;
        left: 0;
        right: 0;
        z-index: 100;
        .login_area{
            position: absolute;
            top: 9px;
            left: 12px;
            .user_Login{
                display: block;
                height: 30px;
                line-height: 30px;
                margin-top: 17px;
                font-size: 28px;
                color: #666;
            }
        }

        .header_logo{
            display: block;
            width: 210px;
            margin: 22px auto;
        }
        .download_btn{
            position: absolute;
            min-width: 120px;
            height: 56px;
            line-height: 56px;
            font-size: 24px;
            padding: 0;
            margin-top: -28px;
            border-radius: 4px;
            border-width: 0;
            top: 50%;
            right: 12px;
        }
    }
</style>
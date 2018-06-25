<template lang="html">
    <div class="home">
        <HomeHeader></HomeHeader>
        <MoneySlider></MoneySlider>
        <MoneyAda></MoneyAda>
        <Money></Money>
        <MoneyAdb></MoneyAdb>
        <MoneyFinance></MoneyFinance>
        <MoneyAdc></MoneyAdc>
        <HomeFooter cname="mfooter"></HomeFooter>
        <HomeNavbar></HomeNavbar>
    </div>
</template>

<script>
    import HomeHeader from '../public/header'
    import HomeFooter from '../public/footer'
    import HomeNavbar from '../public/navbar'
    import MoneySlider from './moneyslider'
    import MoneyAda from './ada'
    import MoneyAdb from './adb'
    import MoneyAdc from './adc'
    import Money from './money'
    import MoneyFinance from './finance'

    export default {
        components: {
            HomeHeader,
            MoneySlider,
            HomeFooter,
            HomeNavbar,
            MoneyAda,
            MoneyAdb,
            MoneyAdc,
            Money,
            MoneyFinance
        }
    }
</script>

<style lang="scss" type="text/scss">
    @import '../../css/reset.scss';
    .mfooter {
        ul{
            li:first-child{
                display: none;
            }
        }
    }
</style>

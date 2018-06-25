<template lang="html">
    <div class="home">
        <HomeHeader></HomeHeader>
        <HomeSlider></HomeSlider>
        <HomeNovice></HomeNovice>
        <HomeBorrow></HomeBorrow>
        <HomeMoney></HomeMoney>
        <HomeProduct></HomeProduct>
        <HomeLife></HomeLife>
        <HomeFooter></HomeFooter>
        <HomeNavbar></HomeNavbar>
    </div>
</template>

<script>
    import HomeHeader from '../public/header'
    import HomeFooter from '../public/footer'
    import HomeNavbar from '../public/navbar'
    import HomeSlider from './homeslider'
    import HomeNovice from './novice'
    import HomeBorrow from './borrow'
    import HomeMoney from './money'
    import HomeProduct from './product'
    import HomeLife from './life'
    export default {
        components: {
            HomeHeader,
            HomeSlider,
            HomeNovice,
            HomeBorrow,
            HomeMoney,
            HomeProduct,
            HomeLife,
            HomeFooter,
            HomeNavbar
        }
    }
</script>

<style lang="scss" module>
    @import '../../css/reset.scss';
</style>

<template lang="html">
    <div class="home">
        <HomeHeader></HomeHeader>
        <IousSlider></IousSlider>
        <IousWelfare></IousWelfare>
        <IousService></IousService>
        <HomeFooter></HomeFooter>
        <HomeNavbar></HomeNavbar>
    </div>
</template>

<script>
    import HomeHeader from '../public/header'
    import HomeFooter from '../public/footer'
    import HomeNavbar from '../public/navbar'
    import IousSlider from './islider'
    import IousWelfare from './welfare'
    import IousService from './service'
    export default {
        components: {
            HomeHeader,
            HomeFooter,
            HomeNavbar,
            IousSlider,
            IousWelfare,
            IousService
        }
    }
</script>

<style lang="scss">
    @import '../../css/reset.scss';
</style>

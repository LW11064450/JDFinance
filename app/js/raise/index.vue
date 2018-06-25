<template lang="html">
    <div class="home">
        <HomeHeader></HomeHeader>
        <rslider></rslider>
        <daily></daily>
        <In></In>
        <more></more>
        <HomeFooter></HomeFooter>
        <HomeNavbar></HomeNavbar>
    </div>
</template>

<script>
    import HomeHeader from '../public/header'
    import HomeFooter from '../public/footer'
    import HomeNavbar from '../public/navbar'
    import rslider from './rslider'
    import daily from './daily'
    import  In  from './in'
    import  more  from './more'
    export default {
        components: {
            HomeHeader,
            HomeFooter,
            HomeNavbar,
            rslider,
            daily,
            In,
            more
        }
    }
</script>

<style lang="scss" module>
    @import '../../css/reset.scss';
</style>

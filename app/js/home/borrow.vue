<template>
    <Panel title="极速借贷">
        <div :class="$style.borrow_img">
            <img src="//img12.360buyimg.com/jrpmobile/jfs/t12721/42/2497849749/26333/ec584be4/5a421756N2416c88f.png?width=750&height=280" alt="">
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
    .borrow_img{
        height: 0;
        padding-bottom: 37.3333%;
        overflow: hidden;
        img{
            width: 100%;
        }
    }
</style>
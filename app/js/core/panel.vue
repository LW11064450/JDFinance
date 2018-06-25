<template>
    <div :class="[panelClass,cname]">
        <h4>-{{title}}-</h4>
        <slot></slot>
    </div>
</template>

<script type="text/ecmascript-6">
    export default {
        name: "Panel",
        props: {
            cname: String,
            title: String
        },
        data () {
            return {
                panelClass: "panel"
            }
        }
    }
</script>

<style lang="scss" type="text/scss">
    @import "../../css/element.scss";
    .panel{
        @include panel;
    }
</style>
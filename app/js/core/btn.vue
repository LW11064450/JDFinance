<template>
    <div :class="[btn,cname]">
        <slot></slot>
    </div>
</template>

<script type="text/ecmascript-6">
    export default {
        name: "Btn",
        props:{
            cname: String
        },
        data () {
            return {
                btn: "btn"
            }
        },
    }
</script>

<style lang="scss">
    @import "../../css/element.scss";
    .btn{
        @include btn;
    }
</style>
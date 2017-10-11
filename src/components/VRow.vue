<script>
    export default {
        props: {
            backgroundColor: {
                type: String,
                default: ''
            }
        }
    };
</script>

<template>
    <div class="row" :class="backgroundColor">
        <slot></slot>
    </div>
</template>

<style scoped lang="scss">
    .row {
        &.gray {
            background: #e3e3e3;
        }
    }
</style>
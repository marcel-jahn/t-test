<script>
    export default {
        props: {
            item: {
                required: true
            }
        },
        computed: {},
        methods: {
            showFeature() {
                alert(this.item.text);
            }
        }
    };
</script>

<template>
    <div class="Feature" @click="showFeature">
        <div class="Feature__content">
            <div class="Feature__icon" :class="item.name"></div>
            <div class="Feature__text">{{ item.text }}</div>
            <div class="Feature__description">{{ item.description }}</div>
        </div>
    </div>
</template>

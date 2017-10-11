<script>
    import Downloads from './Downloads';

    export default {
        components: {
            Downloads
        }
    };
</script>

<template>
    <header class="Header">
        <div class="Header__content">
            <div class="Header__logo"><img src="../assets/img/logo.png"></div>
            <div class="Header__text"><span>A great new free psd theme to showcase your new application.</span>
            </div>
            <downloads class="Header__downloads"></downloads>
        </div>
    </header>
</template>

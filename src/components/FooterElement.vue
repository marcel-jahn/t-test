<script>
    export default {
        mounted() {
            console.log('Zeit wurde knapp, sorry :)');
        }
    };
</script>

<template>
    <footer class="Footer container">
        <ul class="Footer__items">
            <li class="Footer__item"><a href="#">Contact</a></li>
            <li class="Footer__item"><a href="#">Download</a></li>
            <li class="Footer__item"><a href="#">Press</a></li>
            <li class="Footer__item"><a href="#">Email</a></li>
            <li class="Footer__item"><a href="#">Support</a></li>
            <li class="Footer__item"><a href="#">Privacy</a></li>
        </ul>
    </footer>
</template>

<style scoped lang="scss">
    .Footer {
        &__item {
            display: inline-block;
            margin-right: 35px;
            a {
                color: #848484;
                text-decoration: none;

                &:hover {
                    color: darken(#848484, 10%);
                }
            }
        }

        @media only screen and (max-width: 768px) {

            &__items {
                display: flex;
                flex-wrap: wrap;
                width: 100%;
                align-items: center;
                justify-content: center;
            }

            &__item {
                width: 50%;
                display: block;
                margin: 0 0 30px;
            }
        }
    }
</style>
<script>
    import NewsletterSignup from './NewsletterSignup';

    export default {
        components: {
            NewsletterSignup
        },
        methods: {
            signedUp(emailAdress) {
                alert(`${emailAdress} signed up!`);
            }
        }
    };
</script>

<template>
    <div class="Marketing container">

        <newsletter-signup class="Marketing__newsletter" @on-sign-up="signedUp"></newsletter-signup>

        <div class="Marketing__video">
            <iframe src="https://player.vimeo.com/video/237748768"
                    frameborder="0"
                    webkitallowfullscreen
                    mozallowfullscreen
                    allowfullscreen></iframe>
        </div>

    </div>
</template>

<style lang="scss" scoped>
    .Marketing {
        display: flex;
        justify-content: space-between;
        text-align: left;

        &__video {
            width: 500px;
            height: 300px;
            border-radius: 20px;
            overflow: hidden;

            iframe {
                width: 100%;
                height: 100%;
            }
        }
        &__newsletter {
            padding-right: 30px;
        }

        @media only screen and (max-width: 768px) {
            display: block;

            &__newsletter {
                margin-bottom: 30px;
                padding: 0;
            }

            &__video, &__newsletter {
                width: 100%;
            }
        }
    }
</style>

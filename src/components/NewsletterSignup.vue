<script>
    export default {
        data() {
            return {
                email: ''
            };
        },
        methods: {
            onSignUp() {
                if (this.email.length)
                    this.$emit('on-sign-up', this.email)
            }
        }
    };
</script>

<template>
    <div class="Newsletter-signup">
        <h2>Get Notified Of Any Updates!</h2>

        <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse fringilla fringilla nisl congue congue. Maecenas nec condimentum libero, at elementum mauris. Phasellus eget nisi dapibus, ultricies nisl at, hendrerit risusuis ornare luctus id sollicitudin ante lobortis at.
        </p>

        <div class="Newsletter-signup__input-wrap">
            <input class="Newsletter-signup__input" placeholder="Email Adress" v-model="email">

            <button class="Newsletter-signup__button btn"
                    @click="onSignUp"
            >
                Notify
            </button>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    .Newsletter-signup {
        max-width: 540px;


        &__input-wrap {
            border-radius: 15px;
            border: 1px solid #c8c8c8;
            overflow: hidden;
            display: flex;
            height: 55px;
            max-width: 445px;
        }

        &__input {
            font-size: 18px;
            padding: 15px 25px;
            border: 0;
            outline: 0;
            flex-grow: 1;
        }

        &__button {
            color: #fff;
            background: #2ecc71;
            padding-right: 48px;

            &:hover {
                background: darken(#2ecc71, 5%)
            }

            &:active {
                background: darken(#2ecc71, 10%)
            }
        }
    }
</style>
<script>
    import Downloads from './Downloads';
    import Features from './Features/Index';
    import VRow from './VRow';
    import Marketing from './Marketing';
    import FooterElement from './FooterElement';

    export default {
        components: {
            VRow,
            Downloads,
            Features,
            Marketing,
            FooterElement
        }
    };
</script>

<template>
    <div class="Home">
        <div class="Header">
            <div class="Header__content">
                <div class="Header__logo"><img src="../assets/img/logo.png"></div>
                <div class="Header__text"><span>A great new free psd theme to showcase your new application.</span>
                </div>
                <downloads class="Header__downloads"></downloads>
            </div>
        </div>

        <div class="content">
            <v-row>
                <features></features>
            </v-row>
            <v-row background-color="gray">
                <marketing></marketing>
            </v-row>
            <v-row>
                <div class="team-social container">
                    <p class="quote">
                        “Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris interdum velit vitae nulla molestie eu commodo nulla dapib us. Donec id sollicitudin urna. Integer at dui ac leo fermentum varius eleifend ut.”
                    </p>

                    <h2>Say Hi & Get in Touch</h2>

                    <p>
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit suspendisse.
                    </p>
                </div>
            </v-row>
            <v-row background-color="gray">
                <footer-element></footer-element>
            </v-row>
        </div>
    </div>
</template>

<script>
    import Features from './Features/Index';
    import VRow from './VRow';
    import Marketing from './Marketing';
    import HeaderElement from './HeaderElement';
    import FooterElement from './FooterElement';
    import TeamSocial from './TeamSocial';

    export default {
        components: {
            VRow,
            Features,
            Marketing,
            FooterElement,
            TeamSocial,
            HeaderElement
        }
    };
</script>

<template>
    <div class="Home">

        <header-element></header-element>

        <div class="content">

            <v-row>
                <features></features>
            </v-row>

            <v-row background-color="gray">
                <marketing></marketing>
            </v-row>

            <v-row>
                <team-social></team-social>
            </v-row>

            <v-row background-color="gray">
                <footer-element></footer-element>
            </v-row>

        </div>
    </div>
</template>

<script>
    import Feature from './Feature';

    export default {
        components: {
            Feature
        },
        computed: {
            features() {
                return [
                    {
                        name: 'editable',
                        text: 'Editiable Theme',
                        description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse fringilla fringilla.',
                        href: '#'
                    },
                    {
                        name: 'flat',
                        text: 'Flat Design',
                        description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse fringilla fringilla.',
                        href: '#'
                    },
                    {
                        name: 'reach',
                        text: 'Reach Your Audience',
                        description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse fringilla fringilla.',
                        href: '#'
                    },
                ];
            }
        }
    };
</script>

<template>
    <div class="Features container">
        <feature v-for="feature in features"
                 :item="feature"
                 :key="feature.name"
        ></feature>
    </div>
</template>

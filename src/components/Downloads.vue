<script>
    export default {
        computed: {
            platforms() {
                return [
                    {
                        name: 'Apple',
                        link: '#apple-download',
                    },
                    {
                        name: 'Android',
                        link: '#android-download',
                    },
                    {
                        name: 'Windows',
                        link: '#windows-download',
                    },
                ];
            }
        }
    };
</script>

<template>
    <div class="Downloads">
        <a class="Downloads__item"
           v-for="platform in platforms"
           :href="platform.link"
           :title="platform.name"
           :class="platform.name.toLowerCase()"
        >
            {{ platform.name }}
        </a>
    </div>
</template>

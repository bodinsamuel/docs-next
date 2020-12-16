<template>
    <div id="search"></div>
</template>

<script>
export default {
    name: 'AlgoliaSearchNetlify',
    mounted() {
        this.initialize();
    },
    methods: {
        initialize() {
            algoliasearchNetlify({
                appId: '3WRMIAN5UX',
                apiKey: 'ee6bde21a49208a8bba73955a6c7ea6a',
                siteId: '66959682-80a1-4560-9a5b-2775fe6d35b3',
                branch: 'master',
                selector: 'div#search',
            });
        }
    }
}
</script>

<style>
.aa-Autocomplete, .aa-Panel {
    --color-mark: #3fb983;
    --color-background: #f8f8f!;
    --color-selected: #fff;
    --color-text: #23263b;
    --color-input-icon: #777;
    --color-source-icon: rgba(80,80,80,0.32);
    --height: 1.8rem;
    --height-icon: 1rem;
    --font-size: 0.85rem;
}

.aa-Form {
    margin: 2px 16px 0 0;
}
.aa-InputWrapper {
    border-radius: 16px;
}
.aa-Input {
    box-shadow: none;
}
.aa-Panel {
    position: fixed;
    margin: 12px 0 0 0;
}
</style>
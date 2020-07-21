<template>
   <button class="button button--red" @click="incrementCount">Cliqué {{count}} fois</button>
</template>

<script>
export default {
    name: 'Button',
    data: function() {
        return {
            count: 0
        }
    },
    methods: {
        incrementCount: function() {
            this.count++;
        }
    }
}
</script>

<style lang="scss">
.button {
    padding: 20px;
    color: white;
    background-color: blue;

    &--red {
        background-color: red;
    }
}
</style>
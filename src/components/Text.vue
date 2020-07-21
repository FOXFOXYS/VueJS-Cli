<template>
    <div id="fuck">
        <input type="text" placeholder="colors" v-model="colorinput">
        <button @click="colorisequals">OK</button>
        <h2 :class="classText">Change my color</h2>
    </div>
</template>

<script>
export default {
    name: "Fuck",
    data: function() {
        return {
            classText: "texte",
            colorinput: ""
        
        }
    },
    methods: {
        colorisequals: function() {
            if(['blue', 'red', 'yellow', 'green', 'gray', 'easteregg'].includes(this.colorinput)) {
                this.classText = `texte texte--${this.colorinput}`
            } else {
                this.classText = `texte`
            }
        }
    }
}
</script>

<style lang="scss">
.texte {
    font-size: 48px;;
    color: black;

    &--blue {
        color: blue;
    }
    &--red {
        color: red
    }
    &--yellow {
        color: yellow
    }
    &--green {
        color: green
    }
    &--gray {
        color: gray;
    }
    &--easteregg {
        color: navy;
        font-size: 50px;
    }
}

</style>
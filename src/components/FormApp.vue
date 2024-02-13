<script>
export default {
    data() {
        return {
            input: 0
        }
    },
    methods: {
        submit(event) {
            this.$emit("increment", event, this.input)
            this.input = 0
        }
    }
}
</script>

<template>
    <form @submit="submit">
        <input type="number" v-model="input">
        <input type="submit">
    </form>
</template>
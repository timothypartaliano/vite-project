<script>
export default {
    props: {
        title: String,
        number: Number
    }
}
</script>

<template>
    <h1>{{ title }}</h1>
    <h1>{{ number }}</h1>
</template>
<template>
    <div>
        <h1>The list:</h1>
        <p v-for="value in valueList">{{ value }}</p>
    </div>
</template>

<script>
    export default {
        name: "History",
        props: ["valueList"]
    }
</script>
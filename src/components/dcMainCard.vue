<script>
export default {
    props: {
        card_data: Object,
    },
}

</script>

<template>
    <li>
        <img :src="card_data.thumb" alt="">
        <h2>{{ card_data.series }}</h2>
    </li>
</template>

<style lang="scss"></style>
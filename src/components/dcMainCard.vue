<script>
export default {
    props: {
        card_data: Object,
    },
}

</script>

<template>
    <div class="mainsec">
        <div class="content">
            <li>
                <img :src="card_data.thumb" alt="">
                <h2>{{ card_data.series }}</h2>
            </li>
        </div>
    </div>
</template>

<style lang="scss"></style>
<script>

import DcMainCard from './dcMainCard.vue';


export default {
    props: {
        cards: Array,

    },
    components: { DcMainCard },
};

</script>

<template>
    <div class="mainsec">
        <div class="content">

            <DcMainCard v-for="card in cards" :card_data="card" />

        </div>
    </div>
</template>

<style lang="scss">
@use "../assets/scss/general.scss" as *;

.mainsec {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;

}



.content li img {
    width: 280px;
    height: 280px;

}

.content h2 {
    font-size: 10px;
}

h1 {
    color: white;
}
</style>
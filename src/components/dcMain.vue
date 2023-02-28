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
        <button class="loadmore">LOAD MORE</button>
    </div>
</template>

<style lang="scss">
@use "../assets/scss/general.scss" as *;


.loadmore {
    background-color: rgb(57, 57, 255);
    color: white;
    margin-bottom: 100px;
}

.mainsec {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
    background-color: black;

}

.content li {
    width: calc(100%/6);
    list-style: none;

}

.content img {
    width: 200px;
    height: 200px;
}

.content h2 {
    font-size: 10px;
    color: white;
}

h1 {
    color: white;
}
</style>
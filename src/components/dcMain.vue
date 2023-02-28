<script>

import comics from "../App.vue";

export default {
    props: {
        card: Object,
    },

    components: { comics },
};


</script>

<template>
    <div class="mainsec">
        <div class="content">
            <!--<h1>..> Content goes here</h1>-->
            <comics v-for="card in comics" />
        </div>
    </div>
</template>

<style lang="scss">
@use "../assets/scss/general.scss" as *;



h1 {
    color: white;
}
</style>
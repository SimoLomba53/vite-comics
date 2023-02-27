<script>
export default {
    data() {
        return {
            itemList: [
                { singleItem: "CHARACTERS" },
                { singleItem: "COMICS" },
                { singleItem: "MOVIES" },
                { singleItem: "TV" },
                { singleItem: "GAMES" },
                { singleItem: "COLLECTIBLES" },
                { singleItem: "VIDEOS" },
                { singleItem: "FANS" },
                { singleItem: "NEWS" },
                { singleItem: "SHOP" },
            ]
        }
    }
}
</script>

<template>
    <div class="headsec">
        <div class="conteiner">
            <div>
                <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <div>
                <ul class="itemList">
                    <li v-for="item in itemList">
                        {{ item.singleItem }}
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style lang="scss">
@use "../assets/scss/general.scss" as *;
@use "../assets/scss/font.scss" as *;
</style>
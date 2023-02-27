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

<style>
.headsec {
    width: 100%;
}

.conteiner {
    display: flex;
    flex-direction: row;
    min-width: 1200px;
    justify-content: space-between;
    align-items: center;
}

.itemList {
    display: flex;
    flex-direction: row;
    gap: 20px;
    list-style: none;
}
</style>
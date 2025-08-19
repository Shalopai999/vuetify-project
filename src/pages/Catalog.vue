<template>
    <div class="container-category">
        <div class="subcategory">
            <h1 class="subcategory__title">Каталог товаров</h1>
            <div class="subcategory__item-container">
                <div class="subcategory__item">
                    <label class="subcategory__item__mobile-title" for="Бытовая техника">
                        <v-icon color="#afafaf" icon="mdi-stove" size="large"></v-icon>
                        <div class="subcategory__item__mobile-name">Бытовая техника</div>
                    </label>
                </div>
                <div class="subcategory__item">
                    <label class="subcategory__item__mobile-title" for="Смартфоны">
                        <v-icon color="#afafaf" icon="mdi-cellphone" size="large"></v-icon>
                        <div class="subcategory__item__mobile-name">Смартфоны</div>
                    </label>
                </div>
                <div class="subcategory__item">
                    <label class="subcategory__item__mobile-title" for="ТВ">
                        <v-icon color="#afafaf" icon="mdi-television" size="large"></v-icon>
                        <div class="subcategory__item__mobile-name">ТВ</div>
                    </label>
                </div>
                <div class="subcategory__item">
                    <label class="subcategory__item__mobile-title" for="ПК">
                        <v-icon color="#afafaf" icon="mdi-laptop" size="large"></v-icon>
                        <div class="subcategory__item__mobile-name">ПК</div>
                    </label>
                </div>
                <div class="subcategory__item">
                    <label class="subcategory__item__mobile-title" for="Офис">
                        <v-icon color="#afafaf" icon="mdi-printer-outline" size="large"></v-icon>
                        <div class="subcategory__item__mobile-name">Офис</div>
                    </label>
                </div>
            </div>
        </div>


    </div>

</template>

<script>

</script>

<style scoped lang="scss">
.container-category {
    padding: 12px 16px;
}

.subcategory {
    &__title {
        margin-left: 4px;
    }

    &__item {
        &__mobile-title {
            display: flex;
            flex-direction: row;
            align-items: center;
            justify-content: flex-start;
            padding: 16px 28px 16px 12px;
            background-color: white;
            margin: 4px;
        }

        &__mobile-name {
            margin-left: 16px;
        }
    }
}
</style>
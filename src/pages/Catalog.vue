<template>
    <div class="container-category">
        <Breadcrumb :breadcrumbItems="breadcrumbItems" />
        <div class="subcategory">
            <h1 class="subcategory__title">Каталог товаров</h1>
            <div class="subcategory__item-container">
                <div class="subcategory__item">
                    <label v-for="item in catalog" class="subcategory__item__mobile-title" :for="item.name">
                        <v-icon color="#afafaf" :icon="item.icon" size="large"></v-icon>
                        <div class="subcategory__item__mobile-name">{{ item.name }}</div>
                    </label>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import { reactive, ref } from 'vue';

const catalog = ref([{
    name: 'Бытовая техника',
    icon: 'mdi-stove'
}, {
    name: 'Смартфоны',
    icon: 'mdi-cellphone'
}, {
    name: 'ТВ',
    icon: 'mdi-television'
}, {
    name: 'ПК',
    icon: 'mdi-laptop'
}, {
    name: 'Офис',
    icon: 'mdi-printer-outline'
}])

const breadcrumbItems = [
    {
        title: 'Главная',
        disabled: false,
        href: '/',
    },
    {
        title: 'Каталог',
        disabled: true,
        href: '/catalog',
    },
]

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
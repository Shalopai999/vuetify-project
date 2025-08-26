<template>
    <div>
        <div class="mobile-footer-menu">
            <nav class="menu-nav">
                <ul class="menu-nav__list">
                    <li v-for="item in footerMenu" class="menu-nav__item">
                        <a :href="item.link" class="menu-nav__link">
                            <v-icon color="#afafaf" :icon="item.iconName" size="large"></v-icon>
                            <span class="menu-nav__title">{{ item.menuItemName }}</span>
                        </a>
                    </li>
                </ul>
            </nav>
        </div>
    </div>
</template>

<script setup>
import { reactive, ref } from 'vue';

const footerMenu = ref([{
    menuItemName: 'Главная',
    iconName: 'mdi-home-outline',
    link: '/'
}, {
    menuItemName: 'Магазины',
    iconName: 'mdi-map-marker-outline',
    link: '/shops'
}, {
    menuItemName: 'Каталог',
    iconName: 'mdi-format-align-left',
    link: '/catalog'
}, {
    menuItemName: 'Корзина',
    iconName: 'mdi-cart-outline',
    link: '/cart'
}, {
    menuItemName: 'Профиль',
    iconName: 'mdi-account-outline',
    link: '/profile'
}])

</script>

<style scoped lang="scss">
.menu-nav {
    position: fixed;
    bottom: 0;
    left: 0;
    box-shadow: 0px -2px 8px rgba(0, 0, 0, .15);
    z-index: 10;
    background-color: #fff;
    width: 100vw;
    margin: 0 auto;
    height: 50px;

    &__title {

        font-style: normal;
        font-weight: normal;
        font-size: 12px;
        line-height: 14px;
        display: block;
        color: #8c8c8c;
    }

    &__list {
        display: flex;
        justify-content: space-around;
        align-items: center;
        list-style: none;
        height: 100%;
    }

    &__link {
        display: flex;
        flex-direction: column;
        text-decoration: none;
        align-items: center
    }

    &__icon {
        height: 22px;
        fill: #afafaf;
        color: #afafaf;
    }
}
</style>
<template>
    <div>
        <div class="mobile-footer-menu">
            <nav class="menu-nav">
                <ul class="menu-nav__list">
                    <li class="menu-nav__item">
                        <a href="/" class="menu-nav__link">
                            <v-icon color="#afafaf" icon="mdi-home-outline" size="large"></v-icon>
                            <span class="menu-nav__title">Главная</span>
                        </a>
                    </li>
                    <li>
                        <a href="/" class="menu-nav__link">
                            <v-icon color="#afafaf" icon="mdi-map-marker-outline" size="large"></v-icon>
                            <span class="menu-nav__title">Магазины</span>
                        </a>
                    </li>
                    <li>
                        <a href="/" class="menu-nav__link">
                            <v-icon color="#afafaf" icon="mdi-format-align-left" size="large"></v-icon>
                            <span class="menu-nav__title">Каталог</span>
                        </a>
                    </li>
                    <li>
                        <a href="/" class="menu-nav__link">
                            <v-icon color="#afafaf" icon="mdi-cart-outline" size="large"></v-icon>
                            <span class="menu-nav__title">Корзина</span>
                        </a>
                    </li>
                    <li>
                        <a href="/" class="menu-nav__link">
                            <v-icon color="#afafaf" icon="mdi-account-outline" size="large"></v-icon>
                            <span class="menu-nav__title">Профиль</span>
                        </a>
                    </li>
                </ul>
            </nav>
        </div>
    </div>
</template>

<script>

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
<template>
    <div>
        <div class="mobile-footer-menu">
            <nav class="menu-nav">
                <ul class="menu-nav__list">
                    <li class="menu-nav__item">
                        <a href="/" class="menu-nav__link">
                            <svg class="menu-nav__icon" xmlns="http://www.w3.org/2000/svg" height="20"
                                viewBox="-2 -2 24 24">
                                <path fill="currentColor"
                                    d="M18 18V7.132l-8-4.8l-8 4.8V18h4v-2.75a4 4 0 1 1 8 0V18h4zm-6 2v-4.75a2 2 0 1 0-4 0V20H2a2 2 0 0 1-2-2V7.132a2 2 0 0 1 .971-1.715l8-4.8a2 2 0 0 1 2.058 0l8 4.8A2 2 0 0 1 20 7.132V18a2 2 0 0 1-2 2h-6z" />
                            </svg>
                            <span class="menu-nav__title">Главная</span>
                        </a>
                    </li>
                    <li>
                        <a href="/" class="menu-nav__link">
                            <svg class="menu-nav__icon" xmlns="http://www.w3.org/2000/svg" height="20"
                                viewBox="0 0 24 24">
                                <path fill="currentColor"
                                    d="M11.5 9A2.5 2.5 0 0 1 14 6.5c1.1 0 2.03.71 2.37 1.69c.08.26.13.53.13.81a2.5 2.5 0 0 1-2.5 2.5c-1.09 0-2-.69-2.36-1.66c-.09-.26-.14-.55-.14-.84M5 9c0 4.5 5.08 10.66 6 11.81L10 22S3 14.25 3 9c0-3.17 2.11-5.85 5-6.71C6.16 3.94 5 6.33 5 9m9-7c3.86 0 7 3.13 7 7c0 5.25-7 13-7 13S7 14.25 7 9c0-3.87 3.14-7 7-7m0 2c-2.76 0-5 2.24-5 5c0 1 0 3 5 9.71C19 12 19 10 19 9c0-2.76-2.24-5-5-5Z" />
                            </svg>
                            <span class="menu-nav__title">Магазины</span>
                        </a>
                    </li>
                    <li>
                        <a href="/" class="menu-nav__link">
                            <svg class="menu-nav__icon" xmlns="http://www.w3.org/2000/svg" height="20"
                                viewBox="0 0 512 512">
                                <path fill="none" stroke="currentColor" stroke-linecap="round" stroke-miterlimit="10"
                                    stroke-width="48" d="M88 152h336M88 256h336M88 360h336" />
                            </svg>
                            <span class="menu-nav__title">Каталог</span>
                        </a>
                    </li>
                    <li>
                        <a href="/" class="menu-nav__link">
                            <svg class="menu-nav__icon" xmlns="http://www.w3.org/2000/svg" height="20"
                                viewBox="0 0 512 496">
                                <path fill="currentColor"
                                    d="M448 69H137l-3-12q-5-23-22.5-37.5T70 5H21q-9 0-15 6T0 27q0 9 6 15t15 6h49q19 0 22 17l49 256q6 21 23.5 34t38.5 13h202q10 0 16-6t6-15q0-22-22-22H203q-14 0-20-12l-2-9h214q20 0 36.5-12t22.5-31l58-123v-5q0-27-18.5-45.5T448 69zm-32 175v2q-3 15-21 15H173l-28-149h303q18 0 21 17zM256 432q0 18-12.5 30.5T213 475q-17 0-29.5-12.5T171 432t12.5-30.5T213 389q18 0 30.5 12.5T256 432zm171 0q0 18-12.5 30.5T384 475t-30.5-12.5T341 432t12.5-30.5T384 389t30.5 12.5T427 432z" />
                            </svg>
                            <span class="menu-nav__title">Корзина</span>
                        </a>
                    </li>
                    <li>
                        <a href="/" class="menu-nav__link">
                            <svg class="menu-nav__icon" xmlns="http://www.w3.org/2000/svg" height="20"
                                viewBox="0 0 24 24">
                                <g fill="none" stroke="currentColor" stroke-width="2">
                                    <path stroke-linejoin="round"
                                        d="M4 18a4 4 0 0 1 4-4h8a4 4 0 0 1 4 4a2 2 0 0 1-2 2H6a2 2 0 0 1-2-2Z" />
                                    <circle cx="12" cy="7" r="3" />
                                </g>
                            </svg>
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
        text-decoration:none;
    }

    &__icon {
        height: 22px;
        fill: #afafaf;
        color: #afafaf;
    }
}
</style>
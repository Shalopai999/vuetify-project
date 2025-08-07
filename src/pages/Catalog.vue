<template>
    <div class="header">
        <div class="header-mobile">
            <div class="header-mobile__back">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 1024 1024">
                    <path fill="#afafaf" d="M224 480h640a32 32 0 1 1 0 64H224a32 32 0 0 1 0-64z" />
                    <path fill="#afafaf"
                        d="m237.248 512l265.408 265.344a32 32 0 0 1-45.312 45.312l-288-288a32 32 0 0 1 0-45.312l288-288a32 32 0 1 1 45.312 45.312L237.248 512z" />
                </svg>
            </div>
            <div class="header-mobile__search">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
                    <path fill="#afafaf"
                        d="M10 4a6 6 0 1 0 0 12a6 6 0 0 0 0-12zm-8 6a8 8 0 1 1 14.32 4.906l5.387 5.387a1 1 0 0 1-1.414 1.414l-5.387-5.387A8 8 0 0 1 2 10z" />
                </svg>
                <input class="header-mobile__input" type="text" placeholder="Поиск по сайту">
                <svg class="header-mobile__scan" xmlns="http://www.w3.org/2000/svg" width="24" height="24"
                    viewBox="0 0 24 24">
                    <path fill="#afafaf" stroke="#afafaf" stroke-linecap="round" stroke-linejoin="round"
                        stroke-width="2"
                        d="M3 7V5a2 2 0 0 1 2-2h2m10 0h2a2 2 0 0 1 2 2v2m0 10v2a2 2 0 0 1-2 2h-2M7 21H5a2 2 0 0 1-2-2v-2M8 7v10m4-10v10m5-10v10" />
                </svg>
            </div>
            <div class="header-mobile__notification">
                <svg class="header-mobile__notification-button" xmlns="http://www.w3.org/2000/svg" width="20"
                    height="20" viewBox="0 0 24 24">
                    <path fill="#afafaf"
                        d="M4 8a8 8 0 1 1 16 0v4.697l2 3V20h-5.611a4.502 4.502 0 0 1-8.777 0H2v-4.303l2-3V8Zm5.708 12a2.5 2.5 0 0 0 4.584 0H9.708ZM12 2a6 6 0 0 0-6 6v5.303l-2 3V18h16v-1.697l-2-3V8a6 6 0 0 0-6-6Z" />
                </svg>
            </div>

        </div>
    </div>
</template>

<script>

</script>

<style scoped lang="scss">
.header {
    min-height: 60px;
    box-shadow: 0 1px 4px #00000029;
}

.header-mobile {

    min-height: 60px;
    padding: 12px 16px;
    gap: 8px;
    display: flex;
    flex-direction: row;
    align-items: center;

    &__back {
        width: 36px;
        height: 36px;
        display: flex;
        justify-content: center;
        align-items: center;
        border-radius: 8px;
        background-color: #f7f7f7;
        flex-shrink: 0;
    }

    &__search {
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 100%;
        height: 36px;
        padding: 0px 8px 0px 8px;
        border-radius: 8px;
        background-color: #f7f7f7;
    }

    &__input {
        width: 100%;
        padding: 0px 8px 0px 8px;
    }

    &__scan {
        padding: 0px 0px 0px 0px;
    }

    &__notification {
        display: flex;
        justify-content: center;
        align-items: center;
        border-radius: 8px;
        background-color: #f7f7f7;
        width: 36px;
        height: 36px;
        flex-shrink: 0;
    }
}
</style>
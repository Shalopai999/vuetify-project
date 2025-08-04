<template>
    <div class="header">
        <div class="header-mobile">
            <div class="header-mobile__back">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 1024 1024">
                    <path fill="currentColor" d="M224 480h640a32 32 0 1 1 0 64H224a32 32 0 0 1 0-64z" />
                    <path fill="currentColor"
                        d="m237.248 512l265.408 265.344a32 32 0 0 1-45.312 45.312l-288-288a32 32 0 0 1 0-45.312l288-288a32 32 0 1 1 45.312 45.312L237.248 512z" />
                </svg>
            </div>
            <div class="header-mobile__search">

            </div>
            <div class="header-mobile__notification">

            </div>

        </div>
    </div>
</template>

<script>

</script>

<style scoped lang="scss">
.header {
    min-height: 60px;
}

.header-mobile {

    min-height: 60px;
    padding: 12px 16px;

    &__back {
        width: 36px;
        height: 36px;
        display: flex;
        justify-content: center;
        align-items: center;
    }
}
</style>
<template>
  <div class="header">
    <div class="header-mobile">
      <div class="header-mobile__back">
        <v-icon color="#afafaf" icon="mdi-arrow-left" size="large"></v-icon>
      </div>
      <div class="header-mobile__search">
        <v-icon color="#afafaf" icon="mdi-magnify" size="large"></v-icon>
        <input class="header-mobile__input" type="text" placeholder="Поиск по сайту">
      </div>
      <div class="header-mobile__notification">
        <v-icon color="#afafaf" icon="mdi-bell-outline" size="large"></v-icon>
      </div>
    </div>
  </div>
  <div class="container-category__breadcrumb">
    <v-breadcrumbs :items="items">
      <template v-slot:divider>
        <v-icon icon="mdi-chevron-right"></v-icon>
      </template>
    </v-breadcrumbs>
  </div>
  <v-app>
    <v-main>
      <router-view />
    </v-main>
  </v-app>
  <MobileFooterMenu />
</template>

<script setup>
const items = [
  {
    title: 'Главная',
    disabled: false,
    href: 'http://localhost:3000/',
  },
  {
    title: 'Каталог',
    disabled: false,
    href: 'http://localhost:3000/catalog',
  },
]
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

.v-main {
  background-color: rgb(246, 246, 246);
}
</style>

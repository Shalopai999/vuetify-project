<template>
        <Breadcrumb  :breadcrumbItems="breadcrumbItems"/>
    <h1>CART</h1>
</template>

<script setup>

const breadcrumbItems = [
    {
        title: 'Главная',
        disabled: false,
        href: '/',
    },
    {
        title: 'Корзина',
        disabled: true,
        href: '/cart',
    },
]

</script>
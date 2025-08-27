<template>
    <div class="footer">
        <v-card class="mx-auto">
            <v-list min-width="300px" max-width="350px" v-model:opened="open">
                <v-list-group value="Company">
                    <template v-slot:activator="{ props }">
                        <v-list-item v-bind="props" title="Компания"></v-list-item>
                    </template>

                    <v-list-item v-for="([title], i) in companyItems" :key="i" :prepend-icon="icon" :title="title"
                        :value="title"></v-list-item>
                </v-list-group>
            </v-list>
            <v-list min-width="300px" max-width="350px" v-model:opened="open">
                <v-list-group value="Client">
                    <template v-slot:activator="{ props }">
                        <v-list-item v-bind="props" title="Покупателям"></v-list-item>
                    </template>

                    <v-list-item v-for="([title], i) in clientItems" :key="i" :prepend-icon="icon" :title="title"
                        :value="title"></v-list-item>
                </v-list-group>
            </v-list>
        </v-card>
        <div class="footer-contacts">
            <p class="footer-contacts__item">
                <a class="footer-contacts__item-link" href="tel:88002000600">8-800-2000-600</a>
            </p>
            <div class="footer-contacts__item">
                <div class="footer-contacts__item-link">Адрес: Пушкина 1</div>
            </div>
            <div class="footer-contacts__copyright">© 2025 Компания</div>
        </div>
    </div>
</template>

<script setup>
import { ref } from 'vue'

const open = ref(['Users'])
const companyItems = [
    ['О компании', 'mdi-plus-outline'],
    ['Новости', 'mdi-file-outline'],
    ['Вакансии', 'mdi-update'],
    ['Политика конфиденциальности', 'mdi-delete'],
]
const clientItems = [
    ['Как оформить заказ', 'mdi-plus-outline'],
    ['Способы оплаты', 'mdi-file-outline'],
    ['Доставка', 'mdi-update'],
    ['Статус заказа', 'mdi-delete'],
    ['Помощь', 'mdi-delete'],
    ['Обратная связь', 'mdi-delete'],
]
</script>

<style scoped lang="scss">
.footer {
    margin-bottom: 50px;
}

.v-card {
    display: flex;
    padding: 12px 16px;
}

.footer-contacts {
    padding: 12px 16px;

    &__item {
        padding: 12px 16px;
    }

    &__item-link {
        color: #8c8c8c;
        text-decoration: none;
    }

    &__copyright {
        color: #8c8c8c;
        padding: 12px 16px;
    }
}
</style>
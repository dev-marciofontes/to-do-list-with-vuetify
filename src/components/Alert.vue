<template>
    <div class="alert-notification">
        <v-alert :text="alertStore.text" :type="alertStore.type" closable
            class="animate__animated animate__pulse"></v-alert>
    </div>
</template>

<script setup>
import 'animate.css';
import { } from '@/store/alert';
const alertStore = useAlertStore();
</script>

<style scoped>
.alert-notification {
    position: fixed;
    z-index: 1;
    bottom: 50px;
    width: 100%;
    padding: 0 35% 0 35%;
}
</style>
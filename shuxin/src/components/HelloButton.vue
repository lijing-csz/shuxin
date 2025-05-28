<template>
    <div>
        <h2>{{ message }}</h2>
        <button @click="changeMessage">点我改文字</button>
    </div>
</template>

<script setup>
import { ref } from 'vue'

const message = ref('你好，Vue！')

function changeMessage() {
    message.value = '你点击了按钮 🎉'
}
</script>

<style scoped>
button {
    padding: 8px 16px;
    font-size: 16px;
}
</style>
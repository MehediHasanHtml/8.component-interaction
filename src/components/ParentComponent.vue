<script setup>
import ChildComponent from './ChildComponent.vue';
import { ref } from 'vue';
const message = ref("Hello World");

</script>

<template>

<h3>ParentComponent</h3>
<p>{{ message }}</p>

<input type="text" placeholder="Type message...." v-model="message">

<ChildComponent v-model="message"></ChildComponent>


</template>

<style scoped>

</style>

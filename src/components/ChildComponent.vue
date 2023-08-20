<script setup>
import { ref } from 'vue';

defineProps(['modelValue'])
defineEmits(['update:modelValue'])

function messageEmitted(){
    return 'Message from childcomponents';  
}

</script>

<template>
<h3>ChildComponent</h3>

<p>{{ message }}</p>
<p>{{ modelValue }}</p>

<hr>

<button @click="$emit('update:modelValue', messageEmitted())"> Button </button>

</template>

<style scoped>

</style>

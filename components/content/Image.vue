<script setup>
defineProps({
  icon: {
    type: String,
    default: 'IconMarkdown'
  }
})
</script>

<template>
    <div>
        <component :is="icon" class=" " />
    </div>
</template>
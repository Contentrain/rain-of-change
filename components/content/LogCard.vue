<template>
  <article v-if="log.publish" class="log-card py-12">
    <log-header
      :tags="log.tags"
      :date="log.relaseDate"
    />
    <ContentRenderer class="prose prose-gray" :value="log" />
  </article>
</template>

<script setup>
// eslint-disable-next-line @typescript-eslint/no-unused-vars
const props = defineProps({
  log: {
    type: Object,
    required: true
  }
})
</script>

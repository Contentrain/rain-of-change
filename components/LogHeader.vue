<template>
  <div class="v-full flex justify-between pb-6">
    <div v-if="tags" class="tags mb-1">
      <Tag
        v-for="tag in tags"
        :key="tag.text + tag.color"
        :tag="tag"
      />
    </div>

    <div class="flex items-end">
      <div class="text-gray-400 text-xs mb-6">
        {{ date }}
      </div>
    </div>
  </div>
</template>

<script setup>
// eslint-disable-next-line @typescript-eslint/no-unused-vars
const props = defineProps({
  date: {
    type: String,
    required: true
  },
  tags: {
    type: Array,
    required: true
  }
})
</script>

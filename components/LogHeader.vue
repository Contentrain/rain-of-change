<template>
  <div class="v-full flex justify-between pb-6">
    <div v-if="versionTags" class="tags mb-1">
      <Tag
        v-for="tag in versionTags"
        :key="tag.text + version"
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
  version: {
    type: String,
    required: true
  },
  date: {
    type: String,
    required: true
  },
  versionTags: {
    type: Array,
    required: true
  }
})
</script>

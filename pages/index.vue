<template>
  <div class="max-w-2xl px-4 m-auto min-h-screen py-24">
    <div v-if="logs && logs.length > 0" class="logs divide-y divide-gray-100">
      <LogCard v-for="log in logs" :key="log.ID" :log="log" />
    </div>
    <div v-else class="w-full text-gray-500 text-center mt-36">
      <h1 class="text-semibold text-xl">
        Ooopss! There are no logs to show.
      </h1>
    </div>
    <div v-if="showButton" class="w-full flex justify-center">
      <button
        class="text-blue-500 text-bold p-2 mt-6 flex justify-start items-center"
        @click="limit += 5"
      >
        Browse all updates <i class="ri-arrow-down-s-line text-2xl ml-2" />
      </button>
    </div>
  </div>
</template>

<script setup lang="ts">
const limit = ref(5)
const { data } = useAsyncData(
  'logs',
  async () => await queryContent('logs').find()
)
const showButton = computed(() => {
  if (data.value?.length > limit.value) {
    return true
  } else {
    return false
  }
})

const logs = computed(() => {
  if (data.value?.length > limit.value) {
    return data.value.slice(
      0,
      limit.value < data.value.length ? limit.value : data.value.length
    )
  } else {
    return data.value
  }
})
</script>

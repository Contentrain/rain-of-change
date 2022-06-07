<template>
  <div class="max-w-2xl px-4 m-auto min-h-screen py-24">
    <div v-if="logs" class="logs divide-y divide-gray-100">
      <LogCard v-for="log in logs" :key="log.version" :log="log" />
    </div>

    <div v-else class="w-full text-center">
      <h1 class="text-semibold text-xl">
        A log records has not been found.
      </h1>
    </div>
    <button v-if="showButton" class="text-blue-500 text-bold p-2 mt-6 flex justify-start items-center" @click="limit += 5">
      Browse all updates <i class="ri-arrow-down-s-line text-2xl ml-2" />
    </button>
  </div>
</template>

<script setup>
const limit = ref(1)
const allLogs = await queryContent('logs').find()
const showButton = computed(() => {
  if (allLogs.length > limit.value) {
    return true
  } else {
    return false
  }
})
const { data } = useAsyncData(
  'logs',
  async () => await queryContent('logs').limit(limit.value).find()
)
const logs = reactive(data)

watch(limit, async () => {
  const data = await queryContent('logs').limit(limit.value).find()
  logs.value = data
})
</script>

<style scoped></style>

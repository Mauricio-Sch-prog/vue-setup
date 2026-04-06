<script setup lang="ts">
defineProps<{
  iDefineTheProps: string,
  notYou: number
}>()
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ iDefineTheProps }}</h1>

    <h3>
      I'm successfully testing vue. numbaa {{ notYou }}
    </h3>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>

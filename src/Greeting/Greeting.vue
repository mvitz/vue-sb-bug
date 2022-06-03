<script>
export default {
  props: {
    /**
     * Greeting.
     */
    greeting: {
      type: String
    },
    /**
     * Color of the text.
     */
    color: {
      type: String,
      default: 'red'
    },
  }
}
</script>

<template>
  <p class="greeting" :style="'color: ' + color + ';'">{{ greeting }}</p>
</template>

<style>
.greeting {
  font-weight: bold;
}
</style>

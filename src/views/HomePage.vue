<template>
  <h1 class="text-red-500 text-[20px]">Hello Home!</h1>
  <p class="count">{{ count }}</p>
  <button class="count-btn" @click="increment">increment</button>
</template>

<script lang="ts">
import { defineComponent, ref } from "vue";

export default defineComponent({
  setup() {
    const count = ref<number>(0);

    const increment = () => {
      count.value++;
    };

    return {
      count,
      increment,
    };
  },
});
</script>

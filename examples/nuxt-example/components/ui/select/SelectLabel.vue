<script setup lang="ts">
import type { HTMLAttributes } from "vue";
import { type SelectLabelProps } from "radix-vue";

const props = defineProps<
	SelectLabelProps & { class?: HTMLAttributes["class"] }
>();
</script>

<template>
  <SelectLabel :class="cn('px-2 py-1.5 text-sm font-semibold', props.class)">
    <slot />
  </SelectLabel>
</template>

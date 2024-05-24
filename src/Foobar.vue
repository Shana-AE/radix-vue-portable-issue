<script setup lang="ts">
import { Primitive, type PrimitiveProps } from 'radix-vue';

export interface Props extends PrimitiveProps {
}

const props = withDefaults(defineProps<Props>(), {
  as: 'button',
});

</script>

<template>
  <Primitive
    :as="as"
  >
    <slot />
  </Primitive>
</template>

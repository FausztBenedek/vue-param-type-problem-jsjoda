<template>
<p>{{ month.toString() }}</p>
</template>

<script lang="ts">
import {defineComponent, type PropType} from "vue";
import type {YearMonth} from "@js-joda/core";

export default defineComponent({
  name: "Inner",
  props: {
    month: {
      type: Object as PropType<YearMonth>,
      required: true,
    }
  }
})
</script>

<style scoped>

</style>

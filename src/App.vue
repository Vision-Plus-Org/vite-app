<template>
  <div>
    <h2-button
      icon="add"
    >
      Click me
    </h2-button>
    <h2-icon
      filename="add_solid"
      button
      color="orange"
    />
    <H2SingleDatePicker
      v-model="date"
      footnote="footnote text"
    />
    <H2DateRangePicker
      v-model="dateRange"
      footnote="footnote text"
    />
  </div>
</template>

<script setup>
import { ref } from 'vue';
import { H2Button, H2Icon, H2SingleDatePicker, H2DateRangePicker } from '@vision-plus-org/vue-ui';

const date = ref('2023-01-01')
const dateRange = ref({ from: '', to: ''})
</script>

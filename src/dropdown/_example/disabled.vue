<template>
  <t-space>
    <t-dropdown :options="options" :min-column-width="112">
      <t-button variant="text">
        <t-space :size="0">
          下拉菜单
          <chevron-down-icon size="16" />
        </t-space>
      </t-button>
    </t-dropdown>
  </t-space>
</template>
<script setup>
import { ChevronDownIcon } from 'tdesign-icons-vue-next';

const options = [
  { content: '选项一', value: 1 },
  { content: '选项二', value: 2 },
  { content: '选项三', value: 3, disabled: true },
  { content: '选项四', value: 4, disabled: true },
];
</script>

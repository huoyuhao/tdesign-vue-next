<template>
  <t-card
    :title="title"
    :subtitle="subtitle"
    :description="description"
    :actions="actions"
    hover-shadow
    :style="{ width: '400px' }"
    @actions="clickHandler"
  >
    {{ infoMessage }}
  </t-card>
</template>
<script setup lang="jsx">
import { MessagePlugin } from 'tdesign-vue-next';

const clickHandler = () => {
  MessagePlugin.success('操作');
};

const title = '标题';
const subtitle = '副标题';
const description = '描述';
const actions = '操作';
const infoMessage = `卡片内容，以描述性为主，可以是文字、图片或图文组合的形式。按业务需求进行自定义组合。`;
</script>

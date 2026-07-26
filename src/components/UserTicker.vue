<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 138****3311 完成了腾讯产品实习生 3 个月转正报告生成"
  },
  {
    "text": "用户 189****7722 生成了字节前端开发实习生转正答辩 8 页大纲"
  },
  {
    "text": "用户 131****9900 完成了新媒体运营实习生 10W+ 爆款成果量化"
  },
  {
    "text": "用户 156****4411 生成了高校校外实习鉴定表优秀导师评语"
  },
  {
    "text": "用户 173****8855 取得了实习期技能提升与业务复盘总结"
  }
]);
</script>

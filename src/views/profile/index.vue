<!--
 * @Author: GZH
 * @Date: 2021-12-07 20:50:59
 * @LastEditors: GZH
 * @LastEditTime: 2022-01-04 15:20:15
 * @FilePath: \vue3-admin-ts\src\views\profile\index.vue
 * @Description:
-->
<template>
  <div>
    {{ $t('msg.login.title') }}

    <el-pagination layout="total, sizes, prev, pager, next, jumper" :total="1000"></el-pagination>
    <el-button>Default</el-button>
    <el-button type="primary">Primary</el-button>
    <el-button type="success">Success</el-button>
    <el-button type="info">Info</el-button>
    <el-button type="warning">Warning</el-button>
    <el-button type="danger">Danger</el-button>
    <el-button @click="changea">中文</el-button>
    {{ aa }}
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'
const aa = ref(111)
const changea = () => {
  aa.value = 123
}
</script>

<style lang="scss" scoped></style>

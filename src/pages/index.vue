<template>
  <div class="wrapper">
    <h1>gitの練習</h1>
    <AppButton btnTitle="次へ" @click="onClickBtn" />
  </div>
</template>

<script lang="ts" setup>
const onClickBtn = () => {
  navigateTo("/practice");
}
</script>

<style lang="scss" scoped>

</style>
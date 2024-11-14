<template>
  <AppButton btnTitle="前へ" @click="onClickBtn" />
</template>
<script lang="ts" setup>
const onClickBtn = () => {
  navigateTo("/");
}
</script>
<style lang="scss" scoped>

</style>
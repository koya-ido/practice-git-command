<template>
  <div>
    <button @click="onClick">{{ Props.btnTitle }}</button>
  </div>
</template>

<script lang="ts" setup>
interface AppButtonProps {
  btnTitle: string;
}

type AppButtonEmits = {
  (event: "click"): void;
};

const Props = withDefaults(defineProps<AppButtonProps>(), {
  btnTitle: "",
});

const emits = defineEmits<AppButtonEmits>();
const onClick = (event: any): void => {
  emits("click");
};
</script>

<style lang="scss" scoped>

</style>
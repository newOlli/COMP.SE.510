<script setup>
import useIcons from "../../../compositionFunctions/useIcons.js";

const props = defineProps({
  emoji: String,
  direction: {
    type: String,
    default: "right",
  },
});
//
const icons = useIcons();
</script>

<template>
  <img :src="icons[props.emoji]" :alt="props.emoji" />
</template>
<style scoped>
img {
  width: 100px;
  height: 100px;
}
</style>

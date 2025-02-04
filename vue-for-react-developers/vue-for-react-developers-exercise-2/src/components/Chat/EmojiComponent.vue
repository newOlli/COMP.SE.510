<script setup>
import Button from "../generic/form/Button.vue";

const emit = defineEmits(["send"]);

function sendEmo(name) {
  emit("send", name);
}
</script>

<template>
  <div>
    <Button icon="shrug" @click="sendEmo('shrug')" />
    <Button icon="octopus" @click="sendEmo('octopus')" />
    <Button icon="mushroom" @click="sendEmo('mushroom')" />
    <Button icon="fire" @click="sendEmo('fire')" />
    <Button icon="tent" @click="sendEmo('tent')" />
  </div>
</template>

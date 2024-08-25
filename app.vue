<template>
  <UAuthForm icon="i-heroicons-face-frown-solid" title="Login" :fields>
    <template #footer>
      <p>Footer: Simple Text</p>
    </template>
  </UAuthForm>
</template>

<script setup lang="ts">
const fields = [
  {
    name: "email",
    type: "email",
    label: "Email",
  },
];
</script>

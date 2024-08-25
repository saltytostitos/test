<template>
  <UPageBody>
    <UContainer class="space-y-8">
      <UAuthForm icon="i-heroicons-user-circle" title="Login" :fields>
        <template #password-hint>
          <UButton disabled variant="link" color="gray"
            >Forgot password?</UButton
          >
        </template>
        <template #footer>
          <div>
            By signing in, you agree to our
            <NuxtLink disabled class="text-primary font-medium"
              >Terms of Service</NuxtLink
            >.
          </div>
        </template>
      </UAuthForm>
    </UContainer>
  </UPageBody>
</template>

<script setup lang="ts">
const fields = [
  {
    name: "email",
    type: "email",
    label: "Email",
  },
  {
    name: "password",
    type: "password",
    label: "Password",
  },
  {
    name: "remember",
    label: "Remember me",
    type: "checkbox",
  },
];
</script>

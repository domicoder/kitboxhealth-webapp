<!-- eslint-disable vue/multi-word-component-names -->
<script setup lang="ts">
  import { useI18n } from 'vue-i18n';

  const { t } = useI18n();
</script>

<template>
  <header class="header">
    <div class="flex flex-col items-center justify-center">
      <p>
        <img
          src="@/assets/images/kitboxhealth-logo-sq.svg"
          alt="logo"
          width="50"
        />
      </p>
      <div class="flex flex-col w-full items-center justify-center">
        <h1 class="text-lg">
          <p class="project-title italic -skew-y-6">
            {{ t('general.appName') }}
          </p>
        </h1>
        <p class="-skew-y-6 pb-4">{{ t('general.appDescription') }}</p>
      </div>
    </div>
  </header>
</template>

<style scoped>
  .project-title {
    color: var(--text-primary-color);
  }
</style>

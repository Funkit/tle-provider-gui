<script setup lang="ts">
defineProps<{
  status: string;
}>();
</script>

<template>
  <div class="layout-topbar">
    <div class="item">
        {{ status }}
    </div>
  </div>
</template>

<style scoped>
.layout-topbar {
  position: fixed;
  height: 5rem;
  z-index: 997;
  left: 0;
  top: 0;
  width: 100%;
  padding: 0 2rem;
  background-color: var(--surface-overlay);
  display: flex;
  align-items: center;
  box-shadow: 0px 3px 5px rgba(0,0,0,.02), 0px 0px 2px rgba(0,0,0,.05), 0px 1px 4px rgba(0,0,0,.08);
}
.layout-topbar .item {
  text-transform: uppercase;
  color:var(--text-color-secondary);
  font-weight: 600;
  margin-bottom: .5rem;
  font-size: .875rem;
}
</style>
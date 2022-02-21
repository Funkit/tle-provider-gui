<script setup lang="ts">
defineProps<{
  title: string;
}>();
</script>

<template>
  <div class="layout-topbar p-component">
    <div class="item logo">
      <img
        alt="Vue logo"
        class="logo"
        src="@/assets/logo.svg"
      />
    </div>
    <div class="item title">
      {{title}}
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
  color:var(--text-color);
  font-weight: 600;
  margin-bottom: .5rem;
  font-size: .875rem;
}

.layout-topbar .logo {
    display: flex;
    align-items: center;
    color: var(--surface-900);
    font-size: 1.5rem;
    font-weight: 500;
    width: 50px;
    border-radius: 12px;
    height: 2.5rem;
    margin-right: .5rem;
}
.layout-topbar .title {
  color:var(--text-color);
  font-weight: 600;
  margin-bottom: .5rem;
  font-size: 1.5rem;
}
</style>
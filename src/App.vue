<script setup lang="ts">
import AppTopBar from "@/components/AppTopBar.vue";
</script>



<template>
  <div>
    <AppTopBar title="TLE Provider" />
    <div class="main-content">
      <div class="grid">
        <Card>
            <template #header>
                This is a header. Can be replaced by a picture
            </template>
            <template #title>
                Advanced Card
            </template>
            <template #content>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Inventore sed consequuntur error repudiandae numquam deserunt
                quisquam repellat libero asperiores earum nam nobis, culpa ratione quam perferendis esse, cupiditate neque quas!
            </template>
            <template #footer>
                <Button icon="pi pi-check" label="Save" />
                <Button icon="pi pi-times" label="Cancel" class="p-button-secondary" style="margin-left: .5em" />
            </template>
        </Card>
      </div>
    </div>
  </div>
</template>

<style>
body {
  color: var(--color-text);
  background: var(--surface-ground);
}
.main-content {
  margin-left: 0;
  padding-left: 2rem;
  padding-right: 2rem;
  padding-top: 2rem;
  margin-top: 5rem;
}
</style>

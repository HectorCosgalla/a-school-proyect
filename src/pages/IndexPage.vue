<template>
  <q-page class="">
    <q-tabs
      v-model="tab"
      align="left"
      active-bg-color="yellow-8"
      class="bg-yellow-7"
      @click="selectedFolder()"
      no-caps
    >
      <q-tab class="folder" name="mails" label="Mails" />
      <q-tab class="folder" name="alarms" label="Alarms" />
      <q-tab class="folder" name="movies" label="Movies" />
    </q-tabs>
    <div class="cube"></div>
  </q-page>
</template>

<script setup>
import { ref } from 'vue'

const tab = ref('mails')
</script>

<style lang="scss">
.folder {
  margin: $space-base * 0.5 $space-base * 0.5 0 $space-base * 0.5;
  border-radius: 20% 20% 0 0;
  box-shadow: $shadow-12;
  padding: 0 $space-base * 3;
}
</style>

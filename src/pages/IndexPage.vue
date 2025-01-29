<template>
  <q-page class="">
    <q-tabs v-model="tab" align="left" active-class="selected-folder" class="bg-amber-3" no-caps>
      <q-tab class="folder" name="mails" label="Mails" />
      <q-tab class="folder" name="alarms" label="Alarms" />
      <q-tab class="folder" name="movies" label="Movies" />
    </q-tabs>
    <q-tab-panels v-model="tab" animated class="shadow-2 rounded-borders">
      <q-tab-panel name="mails">
        <div class="text-h6">Mails</div>
        Lorem ipsum dolor sit amet consectetur adipisicing elit.
      </q-tab-panel>

      <q-tab-panel name="alarms">
        <div class="text-h6">Alarms</div>
        Lorem ipsum dolor sit amet consectetur adipisicing elit.
      </q-tab-panel>

      <q-tab-panel name="movies">
        <div class="text-h6">Movies</div>
        Lorem ipsum dolor sit amet consectetur adipisicing elit.
      </q-tab-panel>
    </q-tab-panels>
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
  background-color: $folder;
}
.selected-folder {
  background-color: $selected-folder;
}
</style>

<template>
  <q-page class="">
    <q-card>
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
    </q-card>
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

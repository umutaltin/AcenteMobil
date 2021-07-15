<template>
  <q-layout view="hHh LpR fFf">
    <q-header class="bg-white text-grey-8 shadow-2">
      <q-toolbar>
        <q-toolbar-title class="row justify-between items-center">
          <q-btn flat icon="keyboard_backspace" />
          Title
          <q-avatar>
            <img src="https://cdn.quasar.dev/img/avatar.png" />
          </q-avatar>
        </q-toolbar-title>
      </q-toolbar>
    </q-header>

    <q-drawer v-model="leftDrawerOpen" side="left" behavior="mobile">
      <!-- drawer content -->
    </q-drawer>

    <q-page-container style="background: #eff3f4">
      <router-view />
    </q-page-container>

    <q-footer class="bg-white shadow-3 text-grey-8">
      <q-toolbar>
        <q-toolbar-title class="row justify-between q-py-md items-center">
          <q-btn round flat icon="home" color="grey-8"  />
          <q-btn round flat icon="people" color="grey-8"  />
          <q-btn round icon="add" text-color="white" color="purple"  />
           <q-btn round flat icon="insights" color="grey-8"  />
          <q-btn round flat icon="notifications" color="grey-8"  />
        </q-toolbar-title>
      </q-toolbar>
    </q-footer>
  </q-layout>
</template>

<script>
export default {
  data() {
    return {
      leftDrawerOpen: false,
    };
  },
};
</script>